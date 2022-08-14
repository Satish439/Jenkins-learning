pipeline{
  agent any
  envirnoment{
    SAMPLE_URL="google.com
  }
   parameters {
          string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

          text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

          booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

          choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

          password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
}

  stages{
   stage('one'){
     steps{
       sh 'echo URL = ${SAMPLE_URL}'
       echo SAMPLE_URL
     }
   }
  }
}