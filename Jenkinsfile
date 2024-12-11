pipeline{
    agent any
    stages{
        stage("Git access"){
            steps{
                script{
                  checkout scm
                }
            }
        }

        stage("Java execution"){
            steps{
                bat 'javac Hello.java'
                bat 'java Hello'
            }
        }

        stage("Python execution"){
            steps{
                bat 'C:\Users\srika\AppData\Local\Microsoft\WindowsApps\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\python.exe py.py'
            }
        }
    }
}
