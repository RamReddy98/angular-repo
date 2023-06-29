pipeline {
    agent {
        label 'jenkins-slave'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Build'
                sh 'npm install'
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                echo 'Test'
                sh 'npm run unit'
            }
        }

        stage('Push') {
            steps {
                echo 'Push'
                sh "npm run deploy"
            }
        }
    }
}