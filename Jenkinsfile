// Jenkinsfile
pipeline {
    agent any
    stages {
        stage('Build Artifacts') {
            steps {
                // Create three files as artifacts
                sh 'echo "artifact 1" > artifact1.txt'
                sh 'echo "artifact 2" > artifact2.txt'
                sh 'echo "artifact 3" > artifact3.txt'
            }
        }
        stage('Archive Artifacts') {
            steps {
                // Archive all three artifacts
                archiveArtifacts artifacts: 'artifact*.txt', allowEmptyArchive: false
            }
        }
    }
}
