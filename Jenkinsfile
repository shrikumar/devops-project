pipeline {
	agent any 
	triggers {
       		 pollSCM '* * * * *'
    	}
	stages {
	stage('Unit Test'){
		steps {
			sh "mvn compile"
			}
		}
		stage ('mvn test') {
			steps {
				sh "mvn test"
			}
		}
		stage('Package'){
			stes {
				sh "mvn package"
			}
		}
	}
}

