node{
   stage('SCM Checkout'){
      git credentialsId: 'GitHubPwd', url: 'https://github.com/satheeshCharles/my-app/'
      git 'https://github.com/satheeshCharles/my-app'
      
   }
   stage('Compile-Package'){
      def mvnHome = tool name: 'maven3', type: 'maven'
      sh "${mvnHome}/bin/mvn package" 
   }
   stage ('BuildDockerImage'){
      sh'docker build -t satheeshcharles/my-app:2.0 .'
}
