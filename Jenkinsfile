pipeline {

   agent any

   stages {
     stage('Clone Repo') {
       steps {
         git 'https://DevOps-Batches@dev.azure.com/DevOps-Batches/DevOps49/_git/rs-cart'
       }
     }
     stage('NPM Install') {
       steps {
         sh label: '', script: '''
         npm install
         '''
       }
     }

     stage('Archieve') {
       steps {
         sh 'tar -czf csrt.tgz node_modules cart.js package.json
        }
    }

  }  

}

