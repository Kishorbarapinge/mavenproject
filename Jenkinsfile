pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/myuser/Documents/software/apache-maven-3.9.6/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/mavenproject.war /home/myuser/Documents/software/apache-tomcat-9.0.86/webapps'
			}}	
}}

