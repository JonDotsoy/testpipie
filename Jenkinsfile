
pipeline {
    agent any
    stages {
        stage('specific') {
            steps {
                sh 'docker run --rm --name MODERN -t -d -u 1000:1000 -w ${PWD} -v ${PWD}:${PWD}:rw -v ${PWD}@tmp:${PWD}@tmp:rw --entrypoint cat node:7.5.0-alpine'
                sh 'env'
            }
        }
    }
}


