pipeline {
    agent any

    stages {
        stage('SubirRepo') {
            steps {
                script {
                    git 'https://github.com/GiulianaAmbrosino/Cloud.git'
                }
            }
        }

        stage('InstalarNode') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('DeployearNode') {
            steps {
                script {
                    sh 'npm start &'
                }
            }
        }
    }
}
