pipeline {
    agent any

    stages {
        stage('Build') {
          steps {
            node {
              checkout scm
              sh 'echo hello'
              def myEnv = docker.build 'mastodon'
              // myEnv.inside {
              //   sh 'make test'
              // }
            }
          }
        }
    }
}
