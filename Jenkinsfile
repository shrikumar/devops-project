pipeline {
	agent any 
	triggers {
       		 pollSCM '*/35 * * * *'
    	}
	stages {
	stage('Unit Test'){
		steps {
			sh "mvn compile"
			}
		}
	}
}

