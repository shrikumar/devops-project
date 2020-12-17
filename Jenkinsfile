pipeline {
	agent any 
	triggers {
       		 cpollSCM '* * * * *'
    	}
	stages {
	stage('Unit Test'){
		steps {
			sh "mvn compile"
			}
		}
	}
}

