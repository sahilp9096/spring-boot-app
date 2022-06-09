

node
{
  stage('SCM Checkout')
  {
      checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '1bd364c1-e9c7-454c-a09c-994a548afe0d', url: 'https://github.com/sahilp9096/spring-boot-app.git']]]
      
  }
  stage('Compile Package')
  {
    
   
    script
    {
      environment
      {
        env.PATH = env.PATH +";c:\\Windows\\System32"
        bat 'mvn spring-boot:run'
        
       }
    }
    
   
  }
  
}
