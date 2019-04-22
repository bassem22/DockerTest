pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                bat "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test" 
            }
        }
        stage('package') { 
            steps {
                bat "mvn package"
            }
        }
          stage('sonar') { 
            steps {
                bat "mvn package sonar:sonar"
            }
        }
    }
}
