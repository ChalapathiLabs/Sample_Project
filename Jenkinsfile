pipeline {
    agent any

    stages {
		
        stage ('Compile Stage') {

            steps {
			dir("/root/.jenkins/workspace/reddy"){
			sh 'mvn clean install'
            }
            }
        }

        
		stage ('Deployment Stage') {

            steps {
                
                    sh 'cp /root/.jenkins/workspace/pipeline/Mavendemo/target/maven-1.0.0.war /root/tomcat/apache-tomcat-9.0.10/webapps/'
              
            }
        }


        
    }
}
