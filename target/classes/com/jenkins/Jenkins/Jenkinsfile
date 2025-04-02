pipeline {
    agent any  // Runs the pipeline on any available Jenkins agent

    stages {
        stage('Clone Repository') {  // Step 1: Pull code from GitHub
            steps {
                git 'https://github.com/your-repo-url.git'  // Change to your repo
            }
        }

        stage('Compile') {  // Step 2: Compile the Java program
            steps {
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run Program') {  // Step 3: Run the program
            steps {
                sh 'java HelloWorld'
            }
        }

        stage('Success Message') {  // Step 4: Print success message
            steps {
                echo 'Build and Execution Successful!'
            }
        }
    }
}
