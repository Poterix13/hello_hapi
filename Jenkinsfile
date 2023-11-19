pipeline {
    agent any

    tools {
        nodejs 'node' // Assurez-vous que l'outil 'node' est configuré dans Jenkins
        docker 'docker' // Assurez-vous que l'outil 'docker' est configuré dans Jenkins
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
