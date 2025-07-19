pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Siva4875/RobotFramework.git'
            }
        }
        stage('Install Requirements') {
            steps {
                bat '"C:\\Users\\Siva Kumar\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\Siva Kumar\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m robot TestCodes'
            }
        }
    }
}
