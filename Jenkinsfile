#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'pgoudreau/docker-maven-node:latest'
        }
      }
      steps {
      	sh 'mvn clean install -X'
      }
    }
  }
}
