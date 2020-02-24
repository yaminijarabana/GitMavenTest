node {
  stage('SCM Checkout') {
        git 'https://github.com/yaminijarabana/GitMavenTest'
        }
   stage('Compile Project'){
     //Get MAVEN HOME PATH
     def mvnHome = tool name: 'Maven 3.6.1', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
       }
 }
