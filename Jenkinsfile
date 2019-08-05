pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('MAKE DIRECTORY') {
            steps {
                sh """
                mkdir /tmp/pipeline
                """
            }
        }
        
        stage('TOUCH NEW FILE') {
            steps {
                sh """
                touch /tmp/pipefile
                """
            }
        }
        
        stage('COPY FILE TO DIR') {
            steps {
                sh """
                cp /tmp/pipefile /tmp/pipeline
                """
            }
        }
    }
}
