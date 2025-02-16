pipeline {
    agent {label 'maven'}
    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }
    stages {
        stage('SCM Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ravdy/tweet-trend-new.git'
            }
        }

        stage('Maven Build') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}