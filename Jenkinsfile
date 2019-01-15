<<<<<<< HEAD
peline {
    agent any
=======
pipeline {
	agent {label 'krishnamastr'}
>>>>>>> ed9049a832e63e0f6495cc45a5f7a767c1ca4f25
    stages {
        stage ('checkout') {
            steps {
                checkout scm
            }
        }
        stage ('Build') {
            steps {
                sh '${m2_home}/bin/mvn -f java-sample-app/pom.xml clean install'
<<<<<<< HEAD
=======
	          }
	}
	    
	    stage ('copy') {
		 steps {
	         sh 'rm -rf /root/etc/puppetlabs/code/environments/production/modules/tomcat/files/*'
		 sh 'mv /home/zippyops/jenkins/workspace/puppetupstream/java-sample-app/target/java-sample-app-1.0.0.war  /etc/puppetlabs/code/environments/production/modules/tomcat/files'
		
		
>>>>>>> ed9049a832e63e0f6495cc45a5f7a767c1ca4f25
            }
        }
    }
}

