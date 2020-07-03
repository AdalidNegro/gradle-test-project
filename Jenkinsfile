#!usr/bin/env groovy
node {
  stage('checkout') {
  checkout scm
     }
stage('Build') {
     sh "chmod +x gradle && ./gradlew clean build"
     }
stage('test') {
     sh "./gradlew clean test"
     }
}
