ile (Declarative Pipeline)

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'apt install npm'
            }
        }
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }

   
}

