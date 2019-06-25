pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3010:3011' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }

    stages {
        stage('TEST') { 
            steps {
                sh 'test.sh' 
            }
    }
}
