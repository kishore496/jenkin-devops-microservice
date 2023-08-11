//SCRIPTED
//DECLARATIVE
pipeline {
	// agent any
	// agent { docker {image 'maven:3.6.3'}}
	agent { docker {image 'node:20-alpine'}}
	stages{
		stage('Build'){
			steps{
				// sh 'mvn --version'
				sh 'node --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	} 
	post {
		always {
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are succsseful'
		}
		failure {
			echo 'I run when you are fail'
		}
		changed {
			echo 'I run when status of the Build changed'
		}
	}
	
}

