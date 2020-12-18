pipeline {
	agent any 
	triggers {
       		 pollSCM '* * * * *'
    	}
	stages {
	if(env.BRANCH_NAME == 'develop') {
	stage('Unit Test'){
		steps {
			sh "mvn compile"
			}
		}
	}
	if(env.BRANCH_NAME == 'staging') {
		stage ('mvn test') {
			steps {
				sh "mvn test"
			}
		}
	}
	if(env.BRANCH_NAME == 'master') {
	stage('Package'){
			steps {
				sh "mvn package"
			}
		}
	}
	
	}
}

