pipeline{
 agent {
   node{
    label 'workstation'
   }
 }
  environment{
    SSH=credentials('SSH')
   }
  parameters {
    string(name: 'COMPONENT', defaultValue:'', descrition: )

  }
  stages{
    stage('Ansible palybook'){
      steps{
        sh
        HOST=$(echo ${COMPONENT} | tr [:lower])
      }
    }
  }
}
