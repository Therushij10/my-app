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
                sh 'echo "rushi123" | sudo -S apt install -y npm
'
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
