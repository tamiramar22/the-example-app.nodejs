pipeline {
	agent any
	stages {
		stage('Build') {
			steps{
			  script {
			    dockerimage = docker.build "tamiramar/zertoimage"
			  }				
			}
		}
		stage('Test'){
			steps{
			  sh "npm run test"  
			}
		}
	}

}
