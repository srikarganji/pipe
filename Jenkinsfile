pipeline {
    agent any
    stages {
        stage("Git access") {
            steps {
                script {
                    // Fetch the source code
                    checkout scm
                }
            }
        }

        stage("Java execution") {
            steps {
                // Compile and run Java program
                bat 'javac Hello.java'
                bat 'java Hello'
            }
        }

        stage("Python execution") {
            steps {
                // Debug: Check if Python is accessible
               echo "hello world from python"
            }
        }
    }
}
