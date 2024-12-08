pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS = credentials('dockerhub-credentials-id')  // Docker Hub credentials ID
        IMAGE_NAME = 'chesh-ire/my-node-app'  // Replace with your Docker Hub repository name
        TAG = 'latest'  // Tag for the image
    }
    stages {
        stage('Clone Repository') {
            steps {
                checkout scm  // Checkout the code from your repository
            }
        }
        stage('Build Docker Image') {
