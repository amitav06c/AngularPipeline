// pipeline {
//    agent { label 'nodejs8' }
//    stages{
//     stage ('checkout'){
//       steps{
//         deleteDir()
//         checkout scm
//       }
//     }

//       agent any
//       agent {
//         docker { image 'node:latest' }
//   }

//     stages {

   //   stage('Checkout external proj') {
//         steps {
//             echo 'Trying to checkoutfrom remote....!!!!!'
//             git branch: '*/main',
//                 credentialsId: 'Personal MacBook Air',
//                 url: 'ssh://git@github.com/amitav06c/AngularPipeline.git'

//             sh "ls -lat"
//                }
//             }

//       stage('Install') {
//         steps {
//           echo 'Trying to install NG dependency....!!!!!'
//           sh "npm install" 
//                }
//             }
//     }
//   stages {
//     stage('Install') {
//       steps { sh 'npm install' }
//     }

//     stage('Test') {
//       parallel {
//         stage('Static code analysis') {
//             steps { sh 'npm run-script lint' }
//         }
//         stage('Unit tests') {
//             steps { sh 'npm run-script test' }
//         }
//       }
//     }

//     stage('Build') {
//       steps { sh 'npm run-script build' }
//     }
//   }
// }

pipeline {
    agent {
        docker { image 'node:10-alpine' }
    }
    stages {
        stage('Restore') {
            steps {
                sh 'npm install'
            }
        }            
    }
}
