pipeline {
    agent any
    stages {
        stage('VerifyDockerVersion') {
            steps {
                sh 'docker -v'
            }
        }
        stage('BuildDocker') {
            steps {
                sh 'docker build -t cloudmagicmaster/nginx:1.3 .'
            }
        }
        stage('PushDocker') {
            steps {
                sh 'docker push cloudmagicmaster/nginx:1.3'
            }
        }
    }
}
