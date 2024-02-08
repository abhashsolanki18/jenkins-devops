pipeline {
	# agent any
	agent { docker {image 'maven:3.6.3'} }
	stages {
		stage ('build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage ('test') {
			steps {
				echo "Test"

			}
		}
		stage ('Integration Test') {
			steps {
				echo "Integration Test"

			}
		} 
	}	
}
