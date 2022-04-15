pipeline {
    agent any
    stages {
        stage('Create a new file') {
            steps {
                // Create a file
                sh "touch ./newfile.txt"
                sh "git add newfile.txt"}
                }
        stage('Commit and push changes to Git') {
            steps {
                sh '''
                git add *
                git commit -m "commit message"
                git push -u origin main --force
                '''
                }
            }
        }
