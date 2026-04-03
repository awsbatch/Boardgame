pipeline {
    agent any
    tools {
        maven 'maven-3.9'
        jdk 'jdk17'
    }
    stages {
        stage('Compile source code') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test Case') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }        
    }
}
