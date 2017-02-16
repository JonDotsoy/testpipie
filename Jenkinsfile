pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'uname -a'
                sh 'ls'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('specific') {
            steps {
                sh 'uname -a'
                sh 'd --version'
                sh 'dc --version'
                sh 'dm --version'
            }
        }
    }
}

