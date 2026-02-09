pipeline {
    agent any

    stages {
        stage('Check Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Run Python App') {
            steps {
                bat 'dir'
                bat 'python main.py'
            }
        }
    }
}
