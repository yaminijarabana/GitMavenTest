node {
  stage('SCM Checkout') {
        git 'https://github.com/yaminijarabana/GitMavenTest'
        }
   stage('Compile Project'){
     //Get MAVEN HOME PATH
     def mvnHome = tool name: 'maven 3.6.3', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
       }
  stage('Email Notification'){
  mail bcc: '', body: '''Hi ,
WELCOME TO JENKINS EMAIL ALERT

Thanks Yamini''', cc: '', from: '', replyTo: '', subject: 'Jenkins pipeline', to: 'jarabanayamini@testingxperts.com,rudrapdas82@gmail.com'
  }  
  
}
