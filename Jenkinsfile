pipeline {
	agent any
	stages {
	
		stage ('One') {
			tools {
               jdk "jdk-1.8.101"
            }
            steps {
                sh 'java -version'
            }
		}
		
		stage ('Build') {
			steps {
			    echo 'Running Build Pipeline'
			    sh 'java -version'
			    /* sh './mvnw -Dmaven.test.failure.ignore=true clean package' */
			    echo 'Completing Build Pipeline'
			}  
		}
		
		stage ('Test') {
		    steps {
			    echo 'Running Test Pipeline'
			}     
		}

	}
}