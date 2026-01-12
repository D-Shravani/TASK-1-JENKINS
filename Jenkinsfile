pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Code cloned from GitHub'
            }
        }

        stage('Compile') {
            steps {
                bat 'javac Calculator.java'
            }
        }

        stage('Run') {
            steps {
                bat 'echo "10 5 +" | java -cp  Calculator'
            }
        }
    }
}
