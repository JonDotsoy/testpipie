pipeline {
    agent { docker 'node' }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }
}