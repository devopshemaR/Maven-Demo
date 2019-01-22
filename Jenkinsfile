pipeline {
    agent any 
    stages{
        stage ("scm"){
        steps {git 'https://github.com/devopshemaR/Maven-Demo.git'}
        }
    stage ("BUILD"){
        steps {bat 'mvn clean '
                bat 'mvn install'}
        }
    
    stage ("Deploy"){
        steps {bat 'xcopy/y "C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline_demo1\\multi-module\\webapp\\target\\webapp.war"  "C:\\Program Files (x86)\\Apache Software Foundation\\Tomcat 8.5\\webapps"'}
        }
    }
    }
