pipeline{
  agent any  
  stages{  
      stage("Run ansible playbook"){
        steps{
        ansiblePlaybook credentialsId: 'ans-key', inventory: 'hosts', playbook: 'nginx_install.yaml'
        }
      }
    stage('print nginx is Installed') {
      steps{
         sh"echo nginx is installed on all servers"
        
      }
      
    }
  }
}
