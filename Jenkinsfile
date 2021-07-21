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
						sh '''
						pwd
						sleep 5
						echo This is the fist stage: DEPLOY
						'''
					}
				}
				stage('test2') {
					steps {
						sh '''
						pwd
						sleep 5
						echo This is the fist stage: DEPLOY
						'''
					}
				}
				stage('test3') {
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
