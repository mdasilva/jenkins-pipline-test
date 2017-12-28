pipeline {
	agent none
	stages {
		stage('Test') {
			agent any
        		steps {
				sh "git -version"
				sh "echo 'hello'"
			}
		}
	}
}

