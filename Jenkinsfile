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
    }
}
