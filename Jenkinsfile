pipeline {
   agent any
   
   stages {
      stage('Clone Sources') {
        steps {
          checkout scm
        } 
      }

      stage('All') {
          steps {
	        script {
	 	    if (env.LANGUAGE == 'All') {
                	echo 'Hello from all languages'
                	echo  'Reading C++ code'
                	sh 'cat C.c'
                	echo 'Reading Python code'
                	sh 'cat PYTHON.py'
                	echo 'Reading Bash code'
                	sh 'cat BASH.sh'
	            }
		    }
		}            
               
    }
	  stage('C') {
            steps {
	          script {
		      if (env.LANGUAGE == 'C') {
			echo 'Hello from C language'
                	echo  'Reading C++ code'
                	sh 'cat C.c'              
	     	       }
		    }
		}                 
    }
	  stage('Bash') {
            steps {
	       script {
	    	   if (env.LANGUAGE == 'BASH') {
	                echo 'Hello from Bash language'
                	echo  'Reading Bash code'
                	sh 'cat BASH.sh'
			    }
	    	}
        }
    }
         stage('Python') { 
            steps {
	        
		script {
		      if (env.LANGUAGE == 'PYTHON') {
		      	echo 'Hello from Python language'
                      	echo  'Reading Python code'
			sh "cat PYTHON.py"
	
           	      }
	         }
            }   
        } 
	  
    }
}
