pipeline {
    agent any

    stages {
        stage('Build') {
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
