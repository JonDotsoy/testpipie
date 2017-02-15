pipeline {
    agent any
    stages {
        stage('install gulp') {
            steps {
                sh 'npm i'
                sh 'npm run gulp'
            }
        }
    }
}

