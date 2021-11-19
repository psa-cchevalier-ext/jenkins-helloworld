node {
    stage('Clone') {
        git 'https://github.com/priximmo/jenkins-helloworld.git'
    }
    stage('Build') {
        sh label: 'Build', script: 'javac Main.java'
    }
    stage('Run') {
        sh label: 'Run', script: 'java Main'
    }
}
