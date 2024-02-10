pipeline {
     
	agent any
	environment{
		dockerHome = tool "myDocker"
		mavenHome = tool "myMaven"
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages {
		stage ('checkout') {
			steps {
				sh 'mvn --version'
				//sh 'docker version'
				sh "java --version"
				echo "Build"
				echo "$PATH"
				echo "Build_no- $env.BUILD_ID"
			}
		}
		stage ('compile') {
			steps {
				sh "mvn clean compile"
			}
		}
		stage ('test') {
			steps {
				//sh "mvn test"

			}
		}
		stage ('Integration Test') {
			steps {
				sh "mvn failsafe:integration-test failsafe:verify"

			}
		} 
	}	
}
