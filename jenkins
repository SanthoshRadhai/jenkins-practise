pipeline{
    agent any
    stages {
        stage('source code') {
            steps {
                echo 'Cloning...'
                   git branch: 'main', url: 'https://github.com/Marvel-k23/jenkins.git'

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'docker build -t job-12 .'
                sh 'docker run -d -p 80:80'
            }
        }
    }
}
