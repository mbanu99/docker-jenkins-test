pipeline {
    agent {
        docker {
            image 'python'
            label 'generic'
        } //docker
    } //agent
    stages {
        stage("Run Hello World") {
            steps {
                sh """
                    cat /etc/hostname
                """
            } //steps
        } //stage
    } //stages
} //pipeline