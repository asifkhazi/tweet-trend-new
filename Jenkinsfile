pipeline {
    agent {label 'maven'}

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
        stage('SCM Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ravdy/tweet-trend-new.git'
            }
        }
    }
}
