pipeline {
	agent any 
	triggers {
       		 pollSCM '* * * * *'
    	}
	
	if(env.BRANCH_NAME == 'develop') {
	stages {
	stage('Unit Test'){
		steps {
			sh "mvn compile"
			}
		}
	}
	}
	if(env.BRANCH_NAME == 'staging') {
	stages {
		stage ('mvn test') {
			steps {
				sh "mvn test"
			}
		}
	}
	}
	if(env.BRANCH_NAME == 'master') {
	stages {
	stage('Package'){
			steps {
				sh "mvn package"
			}
		}
	}
	}
}

