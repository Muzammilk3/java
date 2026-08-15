pipeline {
    agent any

    stages {
        stage('Cloning java github repository') {
            steps {
                git 'https://github.com/Muzammilk3/java.git'
            }
        }
        
        stage('Compile and execute java project') {
            steps {
               bat '''javac Test.java
                      java Test'''
            }
        }
        

