pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                echo 'gitcheckout code ..'
                git 'https://github.com/devopsstephen/artifactory.git'
            }
        }
        stage('package') {
            steps {
                echo 'package'
                sh 'mvn clean package'
            }
        }

}
