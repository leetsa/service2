pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/leegroup1/service.git', credentialsId: 'leetsa')
        git(url: 'https://github.com/leetsa/service2.git', poll: true)
      }
    }

    stage('shell') {
      steps {
        sh 'echo "hello world"'
      }
    }

  }
}