node
{
  stage('SCM Checkout')
  {
        
        git 'https://github.com/sahilp9096/spring-boot-app.git'
  }
  stage('Compile Package')
  {
    def mvn_home = tool name: 'maven', type: 'maven'
    sh "${maven_home}/bin/mvn"
  }
}
