pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scm
            }
        }
        stage('test'){
            steps {
                sh 'npm test'
            }
        }
        stage('build'){
            steps {
                sh 'npm run build'
            }
        }
        stage ('deploy'){
            steps {
                sh 'node index.js'
            }
        }
    }

}
