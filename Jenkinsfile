node
{
  stage('SCM Checkout')
  {
      git 'https://github.com/sahilp9096/spring-boot-app.git'
      git branch: 'main', credentialsId: '1bd364c1-e9c7-454c-a09c-994a548afe0d', url: 'https://github.com/sahilp9096/spring-boot-app.git'
  }
  stage('Compile Package')
  {
    def mvn_home = tool name: 'maven', type: 'maven'
    sh "${mvn_home}/bin/mvn"
  }
}
