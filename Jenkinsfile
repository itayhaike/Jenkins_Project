pipeline {
   agent any
   stages {
      stage('BUILD ALL') {
         steps {
			sh '''
				if [ ${LANGUAGE} == "ALL" ]; then
				echo "The Build is started"
				echo "Build BASH...."
				cat 'BASH.sh'
				echo "Build PYTHON...."
				cat 'PYTHON.py'
				echo "Build c++...."
				cat 'C.c'
				echo "Printd all scripst"
				else 
					echo "anouder choice.."
					
				fi
			'''
         }
      }
	  stage('BASH') { 
         steps {
			sh ''' 
			    if [ ${LANGUAGE} == "BASH.sh" ]; then
			    echo "Build BASH...."
			    cat BASH.sh
			    else
			        echo "anouder choice.."
					exit 0
				fi
			'''
         }
      }
	  stage('PYTHON') {
         steps {
            sh '''
                if [ ${LANGUAGE} == "PYTHON.py" ]; then
			    echo "Build PYTHON...."
			    cat PYTHON.py
			    else
			        echo "anouder choice.."
					exit 0
				fi
			'''
         }
      }
	  stage('C') {
         steps {
            sh '''
                if [ ${LANGUAGE} == "PYTHON.py" ]; then
			    echo "Build PYTHON...."
			    cat PYTHON.py
			    else
			        echo "anouder choice.."
					exit 0
				fi
			'''
        }
      }
   }
}
