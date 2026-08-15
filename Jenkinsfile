pipeline {
    agent any

    stages {
        stage('Cloning java github repo') {
            steps {
                git 'https://github.com/Muzammilk3/java.git'
            }
        }

        stage('Compiling and executing java project') {
            steps {
                sh '''javac Test.java
                java Test'''
            }
        }
    }


    post {
        success {
            mail bcc: '',
                body: 'mail to notify that build is successful',
                cc: 'muzammilahmedk3@gmail.com',
                from: '',
                replyTo: '',
                subject: 'Build successful',
                to: 'muzammilahmedk3@gmail.com'
        }
        failure {
            mail bcc: '',
                body: 'mail to notify that build is failed',
                cc: 'muzammilahmedk3@gmail.com',
                from: '',
                replyTo: '',
                subject: 'Build failure',
                to: 'amuzammilahmedk3@gmail.com'
        }
    }
}

