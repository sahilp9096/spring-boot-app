node
{
  stage('SCM Checkout')
  {
        git 'https://github.com/sahilp9096/spring-boot-app.git'
  }
  Stage('Compile Package')
  {
    def mvn_home = tool name: 'maven', type: 'maven'
    sh "${mvn_home}mvn package"
  }
}
