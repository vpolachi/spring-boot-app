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
                sh '/opt/apache-maven-3.9.9/bin/mvn clean package'
                sh '/opt/apache-maven-3.9.9/bin/mvn test'
            }
        }
    }
}

