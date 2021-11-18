pipeline {
	agent any
	tools {
	
        jdk "jdk-1.8.101"
    }
	stages {
	
		stage ('One') {
			steps {
				echo 'Hi, Test Pipiline'
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