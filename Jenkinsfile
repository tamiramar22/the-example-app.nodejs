pipeline {
	agent any
	stages {
		stage('Build') {
			steps{
			docker build with plugin jenkins include name
			}

		}
		stage('Test'){
			steps{
			docker run -it --name npm test including ports -p 3000 
			}
		}
		stage('Deploy'){
			steps{
			
			}
		}		
	}

}
