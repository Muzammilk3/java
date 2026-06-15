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
    }
    
    
