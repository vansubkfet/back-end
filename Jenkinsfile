pipeline {
	agent any

	stages {
		stage('Build') {
			// agent {
			// 		image 'node:18-alpine'
			// 		reuseNode true
			// 	}
			// }
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