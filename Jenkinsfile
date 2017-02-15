pipeline {
    agent { docker 'node' }
    stages {
        stage('install gulp') {
            steps {
                sh 'npm i'
                sh 'npm run gulp'
            }
        }
    }
}

