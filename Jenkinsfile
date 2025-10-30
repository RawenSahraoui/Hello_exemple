pipeline {
    agent any
    tools {
        jdk 'JDK21'
    }
    stages {
        stage('Checkout code')
        {
            steps {
                git branch: 'main', url: 'https://github.com/RawenSahraoui/Hello_exemple.git'
            }
        }
        stage('Compile code')
        {
            steps {
                sh 'javac Test.java'
            }
        }
        stage('Execute code')
        {
            steps {
                sh 'java Test '
            }
        }
    }
}
