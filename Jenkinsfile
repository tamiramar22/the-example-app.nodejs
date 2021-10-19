pipeline {
	agent {
		docker { image 'node:9'}
	}
	stages {
		stage('Test'){
			steps{
			  sh "npm run test"  
			}
		}
	}
}
