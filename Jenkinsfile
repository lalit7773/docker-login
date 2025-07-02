
pipeline {
       agent any
  stages {
         stage("pull-scm") {
       steps {
      git branch: 'main', url: 'https://github.com/bhimsinghdig/java-test-project.git'
  }
}
 stage("build") {
       steps {
      sh 'sudo mvn clean package'
  }
}
 stage("test") {
       steps {
      sh 'sudo java-jar target/*.jar >  /var/lib/jenkins/workspace/maven-pipeline-job/text.txt'
  }
}
}
}    
