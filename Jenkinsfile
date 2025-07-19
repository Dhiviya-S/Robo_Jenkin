pipeline {
    agent any

    environment {
        PYTHON = '/Library/Frameworks/Python.framework/Versions/3.11/bin/python3'  // Use actual path from `which python3`
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Dhiviya-S/Robo_Jenkin'

            }
        }

        stage('Run Robot Tests') {
            steps {
                sh '"$PYTHON" -m robot TestCodes'
            }
        }
    }
}
