pipeline {
    agent any

stages{
  stage('Build') {
    steps{
//       sh 'g++ -o PES2UG20CS346 PES2UG20CS346_SoumyeJoshi.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS346'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}

