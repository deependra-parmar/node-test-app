pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                nodejs(nodeJSInstallationName: 'Node 8.x', configId: '8.16.1') {
                    sh 'npm config ls'
                }
            }
            steps {
                sh 'npm install' 
            }
            steps{
                sh 'npm run test'
            }
        }
    }
}
