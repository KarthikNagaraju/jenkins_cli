pipeline {
  agent any
    stages {
        stage('Build on k8 ') {
            steps {
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		                    sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install jenkinsprac-app jenkinsprac  --set image.repository=registry.hub.docker.com/karthik1990/samplecode --set image.tag=6'
            }
        }
    }
}