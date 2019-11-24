pipeline{
	agent any
	tools {
		maven 'Maven 3.6.2'
	}
	stages{
		stage ('Clean') {
	 		steps {
				bat 'mvn clean'
	        	}
		}
	 	stage ('Package') {
			steps {
	      		bat 'mvn package'
	        	}	
		}
		stage ('CREATE DOCKER IMAGE') {
			steps {
	      		bat 'mvn install'
	        	}	
		}
	}
}
