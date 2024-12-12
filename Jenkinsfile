pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install my-app age-calculator  --set image.repository=registry.hub.docker.com/amoljorewar/age-calculator --set image.tag=6'
              			
            }           
        }
    }
}
