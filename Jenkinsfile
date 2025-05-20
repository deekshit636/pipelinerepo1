pipeline{
agent any
  environment {
  env1 = "defaults vadue"
}
  stages{
    stage('BUILD'){
      steps{
        echo 'ths ia build projecta'
        echo "this is env variable value: ${env.env1}"
      }
    }
    stage('DEPLOY'){
      steps{
        echo 'deploy stage uanni'
}
}
  }
}
