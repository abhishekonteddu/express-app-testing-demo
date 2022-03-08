#!/bin/groovy
pipeline {
    agent any
  stages {
    stage('Startup') {
      steps {
           sh "pwd"
           dir("${env.WORKSPACE}/express-app-testing-demo") {
           sh "pwd"
           sh 'npm install'
        }
    sh "pwd"
      }
    }
    stage('Test') {
      steps {
          sh "pwd"
           dir("${env.WORKSPACE}/express-app-testing-demo") {
           sh "pwd"
           sh 'npm run test'
        }
      }
    }
    stage('Build') {
      steps {
          sh "pwd"
           dir("${env.WORKSPACE}/express-app-testing-demo") {
           sh "pwd"
           sh 'npm run start&'
           sh 'npm pack'
        }
      }
    }
  }
}
