pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
             echo "javac Test.java"
            }
        }
        stage('run') {
            steps {
              echo "java Test"
            }
        }
    }
    post {

    always  {
        echo "post command execution"
        }
    failure {
                script {
                    echo "failure command execution"
                }
            }
        }
    success{
            script {
                echo "Success command execution"
            }
        }
    }
}
