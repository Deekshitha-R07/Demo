def tomcatWeb = 'C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps'
// def tomcatBin = 'C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\bin'
// def status = ''

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
      
//         stage('Test') {
//             steps {
//                 bat 'mvn test'
//             }
//         }
      
//         stage('Packaging') {
//             steps {
//                 bat 'mvn package'
//             }
//         }
       stage('Deploying') {
            steps {
                sh "copy target\\aespa.war \"${tomcatWeb}\\aespa.war\""
            }
         }
    }
}
