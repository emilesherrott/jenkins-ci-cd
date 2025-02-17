pipeline {
	agent any 
	environment {
		dockerHome = tool "myDocker"
		mavenHome = tool "myMaven"
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	// agent {
		// docker {
			// image 'maven:3.6.3'
			// image 'node:21.7'
		// }
	// }
	stages {
		stage('Checkout') {
			steps {
				echo "env.DOCKER_CERT_PATH"
				// sh 'mvn --version'
				// sh 'docker --version'
				// echo 'Build'
				// echo "Path: $PATH"
				// echo "Buld Number: $env.BUILD_NUMBER"
				// echo "Build ID: $env.BUILD_ID"
				// echo "Build Tag: $env.BUILD_TAG"
				// echo "Build URL: $env.BUILD_URL"
				// echo "Job Name: $env.JOB_NAME"
			}
		}
	}
	post {
		always {
			echo 'I always run'
		}
		success {
			echo 'I run when successful'
		}
		failure {
			echo 'I run when failed'
		}
	}
}