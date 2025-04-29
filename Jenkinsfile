// Jenkinsfile
pipeline {
	agent any
	stages {
		stage('Checkout') {
			steps {
				git url:'https://github.com/PG-NITRINO/AMO_Jenkins_part1.git', branch: 'main'
			}
		}
		stage('Install') {
			steps {
				bat 'pip install -r requirements.txt'
			}
		}
		stage('Test') {
			steps {
				bat 'pytest'
			}
		}
	}
}