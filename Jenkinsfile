pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Ahmedemad190/aws-bootcamp.git'  // Replace with your repository URL
            }
        }
        stage('Run Hello World') {
            steps {
                script {
                    // Assuming the 'hello_world.sh' script is in the root of the repository
                    sh 'chmod +x hello_world.sh'  // Make the script executable (if not already)
                    sh './hello_world.sh'          // Run the Hello World script
                }
            }
        }
    }  