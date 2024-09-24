pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // If it's a Java project using Maven
                    sh 'mvn clean package'
                    // For Docker projects
                    sh 'docker build -t myapp:latest .'
                }
            }
        }
    }
}
