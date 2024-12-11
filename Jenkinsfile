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
                bat '"C:\\Users\\srika\\AppData\\Local\\Microsoft\\WindowsApps\\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\\python.exe" --version'

                // Execute Python script
                bat '"C:\\Users\\srika\\AppData\\Local\\Microsoft\\WindowsApps\\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\\python.exe" py.py'
            }
        }
    }
}
