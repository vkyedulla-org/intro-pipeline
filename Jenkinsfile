pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        echo "Hello ${params.Name}!"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Vamshi'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}