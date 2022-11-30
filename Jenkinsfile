pipeline {
	environment{
		dockerImage= ''
	}
    agent { 
        node {
            label 'shell-agent'
        }
    }
    stages {
        stage('Build') {
            steps {
		script {
	            dockerImage = docker.build 'example'
		    echo dockerImage
		}
            }
        }
    }
}

