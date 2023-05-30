pipeline {
    agent any
    
    stages {

        stage('Checkout') {
            steps {
                // Add build steps here
                checkout scm
            }
        }

        stage('Test') {
            steps {
                // Add test steps here
                echo 'Testing...'
                sh 'mvn test'
            }
        }

        stage('Build') {
            steps {
                // Add build steps here
                echo 'Building...'
                sh 'mvn clean package'
            }
        }
        
        stage('Deploy') {
            steps {
                // Simulated deployment stage with progress updates
                echo 'Deployment in progress...'
                echo '10% of deployment completed.'
                // Perform deployment steps here or simulate with sleep/wait
                sleep 5
                echo '20% of deployment completed.'
                // Additional deployment steps or simulation
                sleep 5
                echo '30% of deployment completed.'
                // More deployment steps or simulation
                sleep 5
                echo 'Deployment done!'
            }
        }
    }
}
