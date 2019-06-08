pipeline {
    agent any 
    tools {
        maven 'Apache Maven 3.6.0'
    stages {
        stage('---clean---') { 
            steps {
                sh 'mvn --version'
                sh 'mvn clean'
            }
        }
        stage('---Test---') { 
            steps {
                sh 'mvn test'
            }
        }
        stage('---package---') { 
            steps {
                sh 'mvn package'
            }
        }
    }
}
}
