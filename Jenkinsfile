
/*pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                 sh 'npm start'
                 sh 'rm -f test-report.xml'
                 sh 'touch test-report.xml'             }
        }
        stage('Test'){
             steps{
                sh 'npm run test'
                echo 'I am going to test it now'
             }
        }
}
       post {
       always {
              junit 'test-report.xml'
           }
  }
}*/

node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'SonarScanner';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
