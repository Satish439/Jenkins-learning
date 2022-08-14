pipeline{

  agent{
    node{
      lable 'workstation'
    }
  }
}

 environment{
    SSH=credentials('SSH')
 }

 parameters{
   string(name: 'COMPONENT', defaultvalue: '', description: 'which Component to run the piprline')

 }

 stages{
   stage('ansible playbook'){
     sh '''
     HOST=$(echo ${COMPONENT} | tr [:lower:] [:upper:])
   }
 }