pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                step{
                    nodejs(nodeJSInstallationName: 'Node 8.x', configId: '8.16.1') {
                        sh 'npm config ls'
                    }
                }

                step {
                    sh 'npm install' 
                }
                step{
                    sh 'npm run test'
                }
            }
        }
    }
}
