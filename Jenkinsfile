pipeline {
    agent { docker 'ruby' }
    stages {
        stages('build') {
            steps {
                sh 'bundle --version'
                sh 'ruby --version'
            }
        }
    }
}
pipeline {
    agent { docker 'node' }
    stages {
        stage('test') {
            steps {
                sh 'echo ok'
                sh 'exit 1' // Error
            }
        }
        stage('build') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }
}