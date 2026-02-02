pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
          stage('Run security tests') {
            steps {
                bat 'npm audit'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run test'
            }
        }
       
    }

}
