pipeline {
    agent any 

    stages {

        stage('Checkout') {
            steps {
                echo "Checkout from git is successfull"
            }
        }

        stage('Install dependencies') {
            steps {
                echo 'Install dependencies successfull'
            }
        }

        stage('Run app.py') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Run unitTest') {
            steps {
                sh 'python3 -m unittest discover'
            }
        }

        stage('deploy code') {
            steps {
                echo "deploy to ECR from feature branch"
            }
        }
    }

}

