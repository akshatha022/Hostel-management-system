pipeline {
    agent any

    stages {
        stage('Check Python') {
            steps {
                bat '"C:\\Users\\User\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" --version'
            }
        }

        stage('Install Requirements') {
            steps {
                bat '"C:\\Users\\User\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Django Check') {
            steps {
                bat '"C:\\Users\\User\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" manage.py check'
            }
        }
    }
}