pipeline {
    agent any

    stages {
        stage('Install') {
            steps {
              sh "npm install -g yarn"
	          sh 'yarn install'
            }
        }

        stage('Build') {
            steps {
	          sh 'yarn run build:all'
            }
        }
    }
}
