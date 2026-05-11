pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/MohsinDevOps552/flask-cicd-project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building Application..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying Application..."'
            }
        }
    }
}
