pipeline {
    agent any
    stages {
        stage("pull-scm") {
            steps {
                git branch: 'main', url: 'https://github.com/lalit7773/docker-login.git'
            }
        }
        stage("build"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}
