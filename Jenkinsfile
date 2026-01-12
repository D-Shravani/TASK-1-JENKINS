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
                sh 'javac src/Calculator.java'
            }
        }

        stage('Run') {
            steps {
                sh 'echo "10 5 +" | java -cp src Calculator'
            }
        }
    }
}
