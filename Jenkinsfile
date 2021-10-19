pipeline {
	agent any
	stages {
		stage('Build') {
			steps{
			  script {
			    dockerImage = docker.build "tamiramar/zertoimage"
			  }				
			}
		}
		stage('Test'){
			steps{
			  sh "docker run --rm dockerImage npm test"  
			}
		}
	}

}
