pipeline {
	agent any
	stages {
		stage('Build') {
			steps{
			  script {
			    dockerImage = docker.build "tamiramar/zertoImage"
			  }				
			}
		stage('Test'){
			steps{
			  script {
			    docker run --rm dockerImage npm test 
			  }
			}
		}
		stage('Deploy'){
			steps{
			
			}
		}		
	}

}
