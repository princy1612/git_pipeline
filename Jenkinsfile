node
{
    stage("checkout scm")
    {
        echo("check the scm")
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '911c2672-2096-4046-9317-a31226659fbc', url: 'https://github.com/princy1612/git_pipeline.git']]])
          }
    stage ("build")
    {
        echo("build the  code")
        bat 'javac BankAppln.java'
    }
    stage ("test")
    {
       
        echo("test the code")
    }
}  
      
       


