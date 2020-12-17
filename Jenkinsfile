pipeline {
	agent any 
	triggers {
       		 cron('* * * * *')
    	}
	stages {
	stage('Unit Test'){
		steps {
			mvn compile
			}
		}
	}
}

