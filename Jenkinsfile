pipeline {
	agent any 
	triggers {
       		 pollSCM '* * * * *'
    	}
	stages {
	stage('Unit Test'){
		when {
			branch 'develop'
		}
		steps {
			sh "mvn compile"
			}
		}
	
	
	stage ('mvn test') {
			when {
				branch 'staging'
			}
			steps {
				sh "mvn test"
			}
		}
	
	stage('Package'){
			when {
				branch 'master'
			}
			steps {
			 
				sh "mvn package"
			}
		}
		
	
	}
}

