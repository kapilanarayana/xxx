pipeline {
    agent any

    stages {
        stage('countinus download') {
            steps {
                git 'https://github.com/boxfuse/boxfuse-sample-java-war-hello.git'
            }
        }
        stage('countinus build') {
            steps {
                sh 'mvn install'
            }
        }
        stage('countinus deployement') {
            steps {
                sh 'cp target/hello-1.0.war /opt/apache-tomcat-9.0.60/webapps'
            }
        }
    }
}

