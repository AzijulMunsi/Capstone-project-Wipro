pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/AzijulMunsi/Employee3_Expense.git'
            }
        }

        stage('Build and Run') {
            steps {
                bat 'docker-compose down'
                bat 'docker-compose up --build -d'
            }
        }
    }
}