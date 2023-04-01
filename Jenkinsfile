#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:ibmjava'
        }
      }
      steps {
      	sh 'mvn clean install -X'
      }
    }
  }
}
