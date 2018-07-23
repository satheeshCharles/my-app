node{
   stage('SCM Checkout'){
     git 'https://github.com/satheeshCharles/my-app'
   }
   stage('Compile-Package'){
      sh 'mvn package'
   }
}
