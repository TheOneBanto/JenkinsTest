pipeline {
    agent { 
        node {
            label 'Test'
            }
      }
    triggers {
        pollSCM '* /5 * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
            	echo "Building stage"
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
            	echo "Test stage"
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
