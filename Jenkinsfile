pipeline {
    agent none
    stages {
        stage('node-14') {
            agent {
                docker { image 'node:14.21.2-alpine'
                args '-p 3000:3000'
                 }
            }
            steps {
                sh 'node --version'
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
}
