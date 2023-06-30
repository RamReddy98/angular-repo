pipeline {
    agent {
        label 'jenkins-slave'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Build'
                sh "npm install"
                sh "npm run build"
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