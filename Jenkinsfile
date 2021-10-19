pipeline {
	agent any 
	stages {
		stage('Build') {
		  steps {
		    script {
		      dockerimage = docker.build "tamiramar22/zerto"
	            }
		  }
		}
		stage('Test'){
			steps{
			  sh "docker run --rm tamiramar22/zerto npm run test"  
			}
		}
	}
}
