def tomcatWeb = 'C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps'
// def tomcatBin = 'C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\bin'
// def status = ''

pipeline {
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages {
        stage('Build') {
            steps {
                sh 'M2_HOME clean install -f Demo/pom.xml'
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
//        stage('Deploying') {
//             steps {
//                 sh "copy target\\aespa.war \"${tomcatWeb}\\aespa.war\""
//             }
//          }
    }
}
