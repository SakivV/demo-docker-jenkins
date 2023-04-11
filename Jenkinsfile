pipeline {
    agent any
    stages {
        stage('Demo') {
            steps {
                echo 'This is demo for Docker-Jenkins integration'
            }
        }
        stage('VerifyDockerVersion') {
            steps {
                sh 'docker -v'
            }
        }
    }
}
