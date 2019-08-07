pipeline {
    agent any
    stages {	
        stage ('Build Stage') {
            steps {
			dir("/var/lib/jenkins/workspace/deploy/"){
			sh 'mvn clean install'
            }
            }
        }
		stage ('Deployment Stage') {
            steps {
                
                    sh 'cp 'cp target/*.war /root/apache-tomcat-9.0.22-src/webapps/'
            }
        }
    }
}
© 2019 GitHub, Inc.
