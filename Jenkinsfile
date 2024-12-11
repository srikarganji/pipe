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
                bat 'python py.py'
            }
        }
    }
}
