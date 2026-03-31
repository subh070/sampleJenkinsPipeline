pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning GitHub repository...'

                // Replace with your GitHub repo URL
                git branch: 'main', url: 'https://github.com/your-username/your-repo.git'
            }
        }
    }

    post {
        success {
            echo 'Checkout completed successfully!'
        }
        failure {
            echo 'Checkout failed. Check logs!'
        }
    }
}
