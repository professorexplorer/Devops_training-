pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
            deleteDir()
            git branch: 'Master', url: 'https://github.com/gshab9/Devops_training-.git'
            }
        }
        
        stage('Build') {
            steps {
                // Execute build commands here
                sh 'cat README.md'
            }
        }
   
        
        stage('Deploy') {
            steps {
                // Execute deployment commands here
                sh 'git status'
            }
        }
    }
    
    // post {
    //     success {
    //         echo 'Pipeline executed successfully!'
    //         // Additional actions for successful build
    //     }
        
    //     failure {
    //         echo 'Pipeline failed!'
    //         // Additional actions for failed build
    //     }
        
    //     always {
    //         // Cleanup steps if needed
    //     }
    // }
}
