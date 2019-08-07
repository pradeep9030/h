pipeline {
    agent any
    stages {	
        stage ('Build Stage') {
            steps {
			dir("cp /var/lib/jenkins/workspace/pipelinejob/"){
			sh 'mvn clean install'
            }
            }
        }
		stage ('Deployment Stage') {
            steps {
                
                    sh 'cp /var/lib/jenkins/workspace/pipelinejob/target/*.war /root/apache-tomcat-9.0.22-src/webapps/'
            }
        }
    }
}
© 2019 GitHub, Inc.
