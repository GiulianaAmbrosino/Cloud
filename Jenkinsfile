pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    git 'https://github.com/GiulianaAmbrosino/Cloud.git'
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    sh 'npm start &'
                }
            }
        }
    }
}
