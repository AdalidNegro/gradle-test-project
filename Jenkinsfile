#!usr/bin/env groovy
node {
    stage('checkout') {
        checkout scm
    }
    stage('Build') {
        sh "chmod +x gradlew && ./gradlew clean build"
    }
    stage('Test') {
        sh "chmod +x gradlew && ./gradlew clean test"
    }
    stage('SonarQube') {
        sh "./gradlew sonarqube"
    }
}



