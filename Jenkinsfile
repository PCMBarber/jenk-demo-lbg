pipeline {

    agent any

    stages {
        stage('Make Folders and files') {
            steps {
                bat '''
                mkdir testingPipeline
                echo "Hi There" > testingPipeline\text.txt
                '''
            }
        }
        stage('View') {
            steps {
                bat '''
                dir
                type testingPipeline\text.txt
                '''
            }
        }
        stage('Run') {
            steps {
                bat 'script.bat'
            }
        }
    }
}
