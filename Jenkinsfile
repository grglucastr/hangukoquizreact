pipeline{
  agent any

  stages{
    stage('Setup repository'){
      steps{
        git(
          branch: 'master',
          credentialId: 'generalkey',
          url: 'git@github.com:grglucastr/hangukoquizreact.git'
        )
      }
    }

    stage('Checkout code'){
      steps{
        checkout scm
      }
    }

    stage('Install Dependencies'){
      steps{
        sh 'yarn install'
      }
    }

    stage('Run Tests'){
      steps{
        echo 'No tests to run'
      }
    }

    stage('Build'){
      steps{
        sh 'yarn build'
      }
    }
  }
}