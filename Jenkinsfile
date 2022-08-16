pipeline {
    agent any
	stages {
		stage('hello') {
			steps{
				echo 'Hello world'
			}
		}
		stage('cat README') {
			when {
				branch 'fix-*'
			}
			steps {
				 sh '''
				 cat README.md
				 '''
			}
		}
	}
}
