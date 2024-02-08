pipeline {
     
	agent { docker {image 'maven:3.9.6-eclipse-temurin-11'} }
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
