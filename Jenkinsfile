pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3010:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('TEST') { 
            steps {
                sh './test.sh' 
            }
	}
    }
}
