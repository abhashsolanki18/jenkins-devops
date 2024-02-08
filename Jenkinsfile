pipeline {
     
	agent any
	stages {
		stage ('build') {
			steps {
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
