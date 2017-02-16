env.CHANGE_AUTHOR = 'root'

pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'set npm_config_cache=npm-cache'
                sh 'set HOME=.'
                sh 'npm install --global gulp'
                sh 'gulp --version'
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


