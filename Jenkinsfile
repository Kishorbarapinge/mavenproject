pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/myuser/Documents/software/apache-maven-3.9.6/bin/mvn install'
	                 }}
            stage('parameter'){
                  steps{
                          parameters {
                                      choice choices: ['DEV', 'QA', 'UAT'], name: 'ENV '
                                       }}}	
}}

