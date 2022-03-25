pipeline {
    agent any
    stages {
        stage('Stage1') {
			parallel {
				stage("Stage 1-A") {
					steps {
						echo 'This is Stage1-A'
						sh 'sleep 5'
					}
				}
				stage("Stage 1-B") {
					steps {
						echo 'This is Stage1-B'
						sh 'sleep 5'
					}
				}
			}
        }
		stage('Stage2') {
			steps {
                echo 'This is Stage2'
				sh 'sleep 5'
            }
        }
    }
}
