
pipeline {
    agent any
    stages {
        stage('make env') {
            steps {
                sh 'docker rm MODERN -f || echo ok'
                sh 'docker run --rm --name MODERN -t -d -w ${PWD} -v ${PWD}:${PWD}:rw -v ${PWD}@tmp:${PWD}@tmp:rw --entrypoint cat node:7.5.0-alpine'
                sh 'docker exec MODERN npm i -g gulp'
            }
        }
    }
}


