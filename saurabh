pipeline {
    agent any
 
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Saurabhjirekar/node-todo-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'docker build -t myapp .'
            }
        }
        stage('Test') {
            steps {
                //this is test
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker run -d --name myapp-container myapp'
            }
        }
    }
}
