pipeline {
    agent any

    stages {
        stage('Checkout code') {
            steps {
                git branch: 'main', url: 'https://github.com/khalkiasma2022/Projet-Java-Jenkins.git'
            }
        }

        stage('Compile code') {
            steps {
                sh 'javac -d bin src/application/Test.java'
            }
        }

        stage('Execute code') {
            steps {
                sh 'java -cp bin application.Test'
            }
        }
    }
}
