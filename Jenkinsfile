pipeline {
    agent any
    
    stages {
        stage('Hello') {
            steps {
                echo "Hello, world!"
            }
        }
        
        stage('Docker') {
            agent {
                docker { image 'node:alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
