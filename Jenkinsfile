pipeline {
    agent any
    stages {
        stage ('Build & PrePod-Deploy') {
            parallel {
                stage('BUILD') {
                    steps {
                        sh 'echo Stage 1: This is a BUILD stage'
                    }       
                }
        
                stage('PrePod-Deploy') {
                    steps {
                        sh 'echo Satge 2: This is PrePod-Deploy'
                    }
                
                }
                
            }
        }    
        stage('Prod-Deployment') {
            steps {
                sh 'echo Satge 3: This is Prod-Deployment'
            }
        }
    }
}
