pipeline {
    agent any
    tools {
        maven 'Maven 3.8.8' // replace with your Jenkins Maven name
    }
    stages {
        stage("Clone Repository") {
            steps {
                git branch: 'main', url: 'https://github.com/lalit7773/docker-login.git'
            }
        }
        stage("Build with Maven") {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}

