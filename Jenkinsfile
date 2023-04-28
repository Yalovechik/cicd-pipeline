pipeline {
  agent any
  stages {
    stage('Check-out') {
      steps {
        git(url: 'https://github.com/Yalovechik/cicd-pipeline.git', branch: 'main')
      }
    }

    stage('Application-build') {
      steps {
        sh '''#!/bin/bash
npm install'''
      }
    }

  }
  environment {
    registry = 'yalovechik/test'
  }
}