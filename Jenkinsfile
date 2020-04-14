pipeline {
    agent {
        dockerfile {
           label 'generic'
        }
    } //agent
    stages {
        stage("Run Hello World") {
            steps {
                sh """
                    python helloworld.py
                """
            } //steps
        } //stage
        stage("Test requests") {
            steps {
                sh """
                    python requestgoogle.py
                """
            } //steps
        } //stage
    } //stages
} //pipeline