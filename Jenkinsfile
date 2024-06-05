pipeline {
    agent {
       node {
         label 'agent_dev1'
      }
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Sahana-sonu/HelloWorldProject.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac Testfile.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java Testfile'
            }
        }
    }
}
