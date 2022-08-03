pipeline {
   agent any
   stages {
       stage('Clone Sources') {
        steps {
          checkout scm
        } 
      }
      stage('BUILD ALL') {
         steps {
			sh '''
			    cd 
				if [ ${LANGUAGE} == ${ALL} ]; then
				echo "The Build is started"
				echo "Build BASH...."
				cat ./BASH.sh
				echo "Build PYTHON...."
				cat ./PYTHON.py
				echo "Build c++...."
				cat ./C.c
				echo "Printd all scripst"
				else 
					echo "anouder choice.."
					
				fi
				echo ${WORKSPACE}
			'''
         }
      }
	  stage('BASH') { 
         steps {
			sh ''' 
			    if [ ${LANGUAGE} == "BASH.sh" ]; then
			    echo "Build BASH...."
			    cat ./BASH.sh
			    else
			        echo "anouder choice.."
				
				fi
			'''
         }
      }
	  stage('PYTHON') {
         steps {
            sh '''
                if [ ${LANGUAGE} == "PYTHON.py" ]; then
			    echo "Build PYTHON...."
			    cat ./PYTHON.py
			    else
			        echo "anouder choice.."
					
				fi
			'''
         }
      }
	  stage('C') {
         steps {
            sh '''
                if [ ${LANGUAGE} == "C.c" ]; then
			    echo "Build C++...."
			    cat ./C.c
			    else
			        echo "anouder choice.."
				
				fi
			'''
        }
      }
   }
}
