pipeline {
	agent none
	stages {
	    stage('do-stuff') {
	    parallel {
		    stage('Test') {
			    agent any
        		    steps {
        		        git url: 'https://github.com/mdasilva/jenkins-pipline-test.git/'
				sh "git --version"
				sh "echo 'hello'"
				echo scm.getUserRemoteConfigs()[0].getUrl()
				sh "start-shell-access.sh"
			    }
		    }
		    stage('Test2') {
		        agent any
		            steps {
		                sh "echo 'this is step 2'"
		           }
		    }
	        }
	    }
	}
}

