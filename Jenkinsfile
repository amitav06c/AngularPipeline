pipeline {
    agent any

    stages {

      stage('Checkout external proj') {
        steps {
            git branch: '*/master',
                credentialsId: 'my_cred_id',
                url: 'ssh://git@github.com:amitav06c/sampleDemo.git'

            sh "ls -lat"
        }
    }
}
