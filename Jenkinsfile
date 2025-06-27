pipeline{
    agent any
    stages{
        stage("pull-scm"){
            steps{
                 git branch: 'main', url: 'https://github.com/lalit7773/maven-project.git'
            }
        }
        stage("build"){
            steps{
                sh 'sudo mvn clean package'
            }
        }
        stage("test"){
            stpes{
                sh 'sudo java -jar target/*.jar >  /var/lib/jenkins/workspace/maven/text.txt'
            }
        }
    }

}
