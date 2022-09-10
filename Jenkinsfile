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

//to take the input(approval) from user to proceed with job in middle sometimes

// pipeline {
//     agent any
//     stages {
//         stage('Example') {
//             input {
//                 message "Should we continue?"
//                 ok "Yes, we should."
//                 submitter "admin"
//                 parameters {
//                     string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//                 }
//             }
//             steps {
//                 echo "Hello, ${PERSON}, nice to meet you."
//             }
//         }
//     }
// }


// pipeline {
//  agent any
//
//  environment {
//    SAMPLE_URL="google.com"
//    SSH = credentials("SSH")
//  }
//
//  parameters {
//    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//
//    text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
//
//    booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
//
//    choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
//
//    password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
//  }
//
//
//  stages {
//
//    stage("One") {
//      steps {
//        sh 'echo URL = ${SAMPLE_URL}'
//        echo SAMPLE_URL
//        echo SSH
//        echo PERSON
//      }
//    }
//
//  }
// }

// to the stages parallel//

// pipeline {
//   agent any
//    stages {
//      stage('S1') {
//        steps {
//          echo 's1'
//       }
//      }
//      stage('s2') {
//        steps {
//          echo 's2'
//        }
//      }
//      stage('Parallel Stages') {
//        when {
//          branch 'main'
//        }
//        parallel {
//          stage('p1') {
//            steps {
//              sh 'sleep120'
//              echo 'p1'
//            }
//          }
//      stage('p2') {
//        steps{
//          echo 'p2'
//          sh 'sleep120'
//        }
//      }
//      stage('p3') {
//        steps {
//         sh 'sleep120'
//         echo 'p3'
//        }
//      }
//        }
//      }
//    }
// }


@Library('roboshop-jenkins-shared-library') _

log.info 'Starting'
log.warning 'Nothing to do!'

COMPONENT = 'cart'

log()