docker.Image.run('-u 1000:1000')

pipeline {
    agent { docker 'node:7.5.0-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'env'
            }
        }
    }
}

// pipeline {
//     agent any
//     stages {
//         stage('specific') {
//             steps {
//                 sh 'ls'
//                 sh 'touch on-any.txt'
//                 sh 'ls'
//             }
//         }
//     }
// }


