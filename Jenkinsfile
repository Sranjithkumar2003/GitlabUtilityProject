pipeline {
	agent any
	
	stages {
	
		stage ('One') {
			steps {
                sh 'java -version'
            }
		}
		
		stage ('Build') {
			steps {
			    echo 'Running Build Pipeline'
			    sh 'java -version'
			    /* sh './mvnw -Dmaven.test.failure.ignore=true clean package' */
			    sh 'mvn -B -DskipTests clean package'
			    echo 'Completing Build Pipeline'
			}  
		}
		
		stage ('Test') {
		    steps {
			    echo 'Running Test Pipeline'
			    sh 'mvn test -Dsurefire.suiteXmlFiles=testng.xml'
			    echo 'Completing Build Pipeline'
			}     
		}

	}
}