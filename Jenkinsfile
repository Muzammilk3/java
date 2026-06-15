pipeline {
    agent any

    stages {
        stage('cloning java repository') {
            steps {
               git 'https://github.com/Sharath-yp25/java.git'
            }
        }
        
        stage('Compiling and executing java project') {
            steps {
               bat '''javac Test.javac
                      java Test'''
            }
        }
        
        
      }
      post{
          scuccess{
              mail bcc: '',
              body: 'ok china build is compleated thankyou',
              cc: 'sidharth2222005@gmail.com',
              from: '',
              replyTo: '',
              subject: 'Build scccess',
              to: 'sidhu2222005@gmail.com'
          }
      }
    }
    
    
