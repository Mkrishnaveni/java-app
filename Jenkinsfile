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
		  
		 mv '/home/zippyops/jenkins/workspace/puppetupstream/java-sample-app/target/java-sample-app-1.0.0.war  /root/'
		
		
            }
        }
    }
}
