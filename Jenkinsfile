node
{
  stage('SCM Checkout')
  {
        
        git branch: 'main', changelog: false, poll: false, url: 'https://github.com/sahilp9096/spring-boot-app.git'
  }
  Stage('Compile Package')
  {
    def mvn_home = tool name: 'maven', type: 'maven'
    sh "${mvn_home}/bin/mvn package"
  }
}
