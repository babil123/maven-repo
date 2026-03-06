pipeline {
    agent any

    tools {
        maven 'Maven-3.9'
        jdk 'Java'
    }

    stages {

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }

    post {
        success {
            echo 'Build and Tests completed successfully!'
        }

        failure {
            echo 'Build or Tests failed!'
        }
    }
}
