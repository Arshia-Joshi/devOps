pipeline {
    agent any
    tools {
        jdk 'JDK21'
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Arshia-Joshi/devOps.git'
            }
        }
        stage('Compile Java') {
            steps {
                bat '''
                javac src\\HelloWorld.java
                '''
            }
        }
        stage('Run Program') {
            steps {
                bat '''
                java -cp src HelloWorld
                '''
            }
        }
    }
}