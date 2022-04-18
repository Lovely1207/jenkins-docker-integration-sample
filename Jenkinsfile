job('NodeJS example') {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven : 'maven-3.8.5'){
                  sh 'mvn clean install'
                }
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                 withMaven(maven : 'maven-3.8.5'){
                  sh 'mvn test'
                }
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                 withMaven(maven : 'maven-3.8.5'){
                  sh 'mvn deploy'
                }
                echo 'Deploying....'
            }
        }
    }
}