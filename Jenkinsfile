pipeline {
  agent any
  stages {
    stage("Build") {
      steps {
        git url: 'https://github.com/saurabhrawat2606/simple-java-maven-app.git'
        withMaven {
          sh "mvn clean verify"
        } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
         }   
   }
}
}
