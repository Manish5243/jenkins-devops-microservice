//scripted


//Declerative
pipeline {
	//agent any
	agent { docker { image 'maven:3.6.3'} }
	stages {
		stage('build') {
			steps {
				//bat 'mvn.cmd --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} 
	post {
		always {
			echo "i run always"
		}
		success {
			echo "i run when you are success"
		}
		failure {
			echo "i run when you fail"
		}
	}

	
}
