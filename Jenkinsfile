pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -c PES1UG20CS479.cpp'
        sh 'g++ -o PES1UG20CS479 PES1UG20CS479.cpp'
        echo 'Build Done Sucessfully'
      }
    }
    stage('Test'){
      steps{
        sh './PES1UG20CS479'
        echo 'Test Done Successfully'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deployment Done Successful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline Failure'
    }
  }
}
    
