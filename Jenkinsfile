pipeline {
     
	agent any
	environment{
		dockerHome = tool "myDocker"
		mavenHome = tool "myMaven"
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages {
		stage ('build') {
			steps {
				sh 'mvn --version'
				sh 'docker version'
				echo "Build"
				echo "$PATH"
				echo "Build_no- $env.BUILD_ID"
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
