pipeline {
	agent {label 'krishnamastr'}
    stages {
        stage ('checkout') {
            steps {
		checkout scm
            }
        }
        stage ('Build') {
            steps {
                sh '${m2_home}/bin/mvn -f java-sample-app/pom.xml clean install'
	          }
	}
	    
	    stage ('copy') {
		 steps {
	         sh 'rm -rf /root/etc/puppetlabs/code/environments/production/modules/tomcat/files/*'
		 sh 'mv /home/zippyops/jenkins/workspace/puppetupstream/java-sample-app/target/java-sample-app-1.0.0.war  /etc/puppetlabs/code/environments/production/modules/tomcat/files'
		
		
            }
        }
    }
}
