node{
   stage('SCM Checkout'){
      git 'https://github.com/satheeshCharles/my-app'
   }
   stage('Compile-Package'){
      def mvnHome = tool name: 'maven3', type: 'maven'
      sh $"(mvnHome)"/bin/mvn package'
   }
}
