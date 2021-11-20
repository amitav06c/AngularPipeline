pipeline {
    agent any

    stages {

   //   stage('Checkout external proj') {
//         steps {
//             echo 'Trying to checkoutfrom remote....!!!!!'
//             git branch: '*/main',
//                 credentialsId: 'Personal MacBook Air',
//                 url: 'ssh://git@github.com/amitav06c/AngularPipeline.git'

//             sh "ls -lat"
//                }
//             }

      stage('Install') {
        steps {
          echo 'Trying to install NG dependency....!!!!!'
          sh 'npm install' 
               }
            }
    }
}
