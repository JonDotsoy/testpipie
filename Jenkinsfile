pipeline {
    agent { docker 'node' }
    stages {
        stage('install gulp') {
            steps {
                sh 'npm i -g gulp'
                sh 'gulp --version'
            }
        }
    }
}

