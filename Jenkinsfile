pipeline {
    agent any
    environment {
        PATH = "/opt/apache-maven-3.8.1/bin/:$PATH"
    }

    stages {
        stage('fetch code from github') {
            steps {
                git 'https://github.com/nihaldevops/JAVA_Spring.git'
            }
        }
        stage('build a package') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('tomcat deploy') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
