pipeline {
	agent {
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
}
