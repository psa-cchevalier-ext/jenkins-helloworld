pipeline {
  agent {
    label 'ecs'
  }
  stages {
    stage('Clone') {
        steps {
            git 'https://github.com/priximmo/jenkins-helloworld.git'
        }
    }
    stage('Build') {
        steps {
            sh label: 'Build', script: 'javac Main.java'
        }
    }
    stage('Run') {
        steps {
            sh label: 'Run', script: 'java Main'
        }
    }
  }
}
