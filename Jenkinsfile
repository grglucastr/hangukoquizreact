pipeline{
  agent any

  stages{
    stage('Checkout code'){
      steps{
        sh 'git clone https://github.com/grglucastr/hangukoquizreact.git'
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