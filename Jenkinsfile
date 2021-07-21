pipeline {
	agent any  
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') {
			parallel {
				stage('test1') {
					steps {
						sh 'sleep 2'
						echo "phase1"
						
					}
				}
				stage('test2') {
					steps {
						sh 'sleep 2'
						echo "phase1"
					}
				}
				stage('test3') {
					steps {
						sh 'sleep 2'
						echo "phase1"
					}
				}
			}	
		}
		
		stage('DEPLOY') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: DEPLOY
				'''
			}	
		}
	}
}
