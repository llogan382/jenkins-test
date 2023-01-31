pipeline {
    agent none
    stages {
        stage('node-14') {
            agent {
                docker { image 'node:14.21.2-alpine' }
            }
            steps {
                sh 'node --version'
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('node-16') {
            agent {
                docker { image 'node:16.19-alpine3.16' }
            }
            steps {
                sh 'node --version'
                                sh 'npm install'
                sh 'npm run build'
            }
        }
                stage('node-18') {
            agent {
                docker { image 'node:18.13-alpine3.17' }
            }
            steps {
                sh 'node --version'
                                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
}
