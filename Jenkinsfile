// /*
// pipeline{
//   agent any
//
// }
//
//  stages{
//    stage('maven version'){
//      steps{
//        sh 'mvn --version'
//      }
//    }
//   } */


pipeline {
 agent any

 environment {
   SAMPLE_URL="google.com"
   SSH = credentials("SSH")
 }

 parameters {
   string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

   text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

   booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

   choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

   password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
 }

 triggers { pollSCM('* * * * *') }

 stages {

   stage("One") {
     steps {
       sh 'echo URL = ${SAMPLE_URL}'
       echo SAMPLE_URL
       echo SSH
       echo PERSON
     }
   }

 }
}
