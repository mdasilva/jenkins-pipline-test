pipeline {
	agent none
	stages {
	    stage('do-stuff') {
	    parallel {
		    stage('Test') {
			    agent any
        		    steps {
				checkout scm
				sh "git --version"
				sh "echo 'hello'"
				sh "start-shell-access.sh"
			    }
		    }
		    stage('Test2') {
		        agent any
		            steps {
				checkout scm
		                sh "echo 'this is step 2'"
		           }
		    }
	        }
	    }
	}
}

