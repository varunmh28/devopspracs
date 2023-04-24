pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/varunmh28/devopspracs.git']]])
      }
    }
    stage('Build') {
      steps {
        sh 'echo "Build step not required for HTML files"'
      }
    }
    stage('Test') {
      steps {
        sh 'echo "Test step not required for HTML files"'
      }
    }
    stage('Deploy') {
      steps {
        sh 'mkdir -p C:\\xampp\\htdocs\\Devops'
        sh 'cp -r *.html C:\\xampp\\htdocs\\Devops'
      }
    }
  }
}
