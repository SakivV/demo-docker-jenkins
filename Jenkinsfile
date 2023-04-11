pipeline {
    agent any
    stages {
        stage('VerifyDockerVersion') {
            steps {
                sh 'docker -v'
            }
        }
        stage('RunDocker') {
            steps {
                sh 'docker run hello-world'
            }
        }
        stage('BuildDocker') {
            steps {
                sh 'docker build -t cloudmagicmaster/nginx:1.0 .'
            }
        }
        stage('PushDocker') {
            steps {
                sh 'docker push cloudmagicmaster/nginx:1.1'
            }
        }
        stage('RunDockerApp') {
            steps {
                sh 'docker run -p 8989:80 -d cloudmagicmaster/nginx:1.1'
            }
        }
    }
}
