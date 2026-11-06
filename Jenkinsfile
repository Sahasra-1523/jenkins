pipeline {
    agent any
    stages {
        stage('Checkout SCM') {
            steps {
                echo 'Checking out source code from GitHub...'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling Java program...'
                bat 'javac HelloWorld.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running Java application tests...'
                bat 'java HelloWorld'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying artifact to target environment...'
            }
        }
    }
}
