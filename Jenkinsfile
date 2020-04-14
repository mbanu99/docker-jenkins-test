pipeline {
    agent {
       dockerfile true
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