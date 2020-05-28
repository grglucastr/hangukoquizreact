pipeline{
  agent any

  tools{
    nodejs 'nodejs14'
  }

  stages{
    stage('Setup repository'){
      steps{
        git(
          branch: 'master',
          credentialsId: 'generalkey',
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

    stage ('List all files in folder'){
      steps{
        sh 'ls -la'
      }
    }
  }
}