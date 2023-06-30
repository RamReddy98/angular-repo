pipeline {
    agent {
        label 'jenkins-slave'
    }

    stages {

        stage('Install') {
            steps {
                echo 'install'
                sh "npm install"
            }
        }

        stage('Build') {
            steps {
                echo 'Build'
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