pipeline{
agent any
  environment {
  env1 = "defaults vadue"
}
  parameters {
  string defaultValue: 'De\\\\fault value', description: 'default value for parameter', name: 'Name', trim: true
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
        echo "Value of parameter 'name' is: ${params.Name}"
}
}
  }
}
