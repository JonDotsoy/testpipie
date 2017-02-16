pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                bash 'ls'
            }
        }
    }
}

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

