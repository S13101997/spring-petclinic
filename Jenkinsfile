#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'nulldriver/maven-resource:2.0.0-rc.18'
        }
      }
      steps {
      	sh 'mvn clean install -X'
      }
    }
  }
}
