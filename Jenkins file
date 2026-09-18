pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Starting Build...'
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Tests...'
                sh 'mvn test'
            }
        }
    }
}
