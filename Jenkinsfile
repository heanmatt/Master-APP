pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Heart') {
            steps {
                echo 'Broken'
            }
        }
        stage('Failing') {
            steps {
                echo 'Push Me'
            }
        }
        stage('Open Chrome') {
            steps {
                // For Windows nodes (uncomment if running on Windows):
                // bat 'start chrome'
                
                // For Linux / WSL nodes:
                sh 'google-chrome &> /dev/null &'
            }
        }
        stage('Shutdown PC') {
            steps {
                // WARNING: This will immediately shut down the machine running the Jenkins agent.
                // For Windows: bat 'shutdown /s /t 0'
                // For Linux: sh 'sudo shutdown -h now'
                echo 'Shutdown command placeholder'
            }
        }
    }
}