node
{
  stage('SCM Checkout')
  {
        
       echo "scm"
  }
  stage('Compile Package')
  {
    def mvn_home = tool name: 'maven', type: 'maven'
    sh "${mvn_home}/bin/mvn"
  }
}
