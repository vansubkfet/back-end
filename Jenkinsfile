pipeline {
	agent any

	stages {
		stage('Build') {
			agent {
					image 'maven:3.8.6'
					reuseNode true
				}
			}
			steps {
				sh '''
					echo "Start to compile Back-End..."
					mvn --version
					mvn -B -DskipTests clean package
				'''
			}
		}
	}
}