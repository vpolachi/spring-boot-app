//Jenkinsfile for Spring boot application


pipeline {
    agent any
    
    stages {
        stage("Checkout code from GitHub") {
            steps {
                git branch: 'main', url: 'https://github.com/vpolachi/spring-boot-app.git'
            }
        }

        stage("Build with Maven") {
            steps {
                echo "Building the application with Maven..."
                sh 'mvn clean package'
            }
        }
    }
}

