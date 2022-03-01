pipeline {
  agent any
  tools {
    maven 'mymaven'
    jdk 'myjdk'
  }
  stages {
    stage ('Clone git') {
      steps {
        git 'https://github.com/chetanamarella/hello-world.git'
      }
    }
    
    stage ('Build war file') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
    
   /* stage ('SSH to Tomcat') {
      steps {
        sshagent(['tomcat']) {
    // some block
}*/
  
