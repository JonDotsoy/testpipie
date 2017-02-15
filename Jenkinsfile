pipeline {
    agent any
    stages {
        stage('specific') {
            steps {
                sh 'd --version'
                sh 'dc --version'
                sh 'dm --version'
            }
        }
    }
}

