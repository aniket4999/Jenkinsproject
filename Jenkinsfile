pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Build the project using Maven
                sh 'mvn clean package'
            }
        }
        stage('Run') {
            steps {
                // Run the Java application..
                sh 'java -cp target/hello-jenkins-1.0-SNAPSHOT.jar HelloJenkins'
            }
        }
    }
}
