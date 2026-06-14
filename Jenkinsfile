pipeline {
    agent any

    stages {

        stage('Code Checkout') {
            steps {
                git 'https://github.com/Suresh5600/Suresh-Repository.git'
            }
        }

        stage('Deploy to Nginx') {
            steps {
                sh 'cp -f /var/lib/jenkins/workspace/Nginx/index.html /usr/share/nginx/html/index.html'
            }
        }
    }
}
