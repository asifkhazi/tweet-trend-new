pipeline {
    agent {label 'maven'}

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
