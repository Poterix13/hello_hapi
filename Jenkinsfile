pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    tools {
        // Utilisez le type d'outil 'jdk' pour Node.js
        nodejs 'node'

        // Utilisez le type d'outil 'dockerTool' pour Docker
        dockerTool 'docker'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
