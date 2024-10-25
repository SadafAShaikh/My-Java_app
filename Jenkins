pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Specify the correct branch name (e.g., 'main' or any other branch)
                git branch: 'main', url: 'https://github.com/SadafAShaikh/My-Java_app.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    bat 'javac Main_1.java'
                }
            }
        }

        stage('Run') {
            steps {
                script {
                    bat'java Main_1'
                }
            }
        }
    }
}
