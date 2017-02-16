
pipeline {
    agent any
    stages {
        stage('specific') {
            steps {
                sh 'd rm MODERN -f || echo ok'
                sh 'docker run --rm --name MODERN -t -d -w ${PWD} -v ${PWD}:${PWD}:rw -v ${PWD}@tmp:${PWD}@tmp:rw --entrypoint cat node:7.5.0-alpine'
                sh 'env'
            }
        }
    }
}


