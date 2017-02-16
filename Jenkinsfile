pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'ls'
                sh 'touch on-node.txt'
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
                sh 'ls'
                sh 'touch on-any.txt'
                sh 'ls'
            }
        }
    }
}

pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'ls'
            }
        }
    }
}

