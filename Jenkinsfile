pipeline {
	agent any
	tools{
		gradle 'Gradle'
	}
	stages{
		stage('checkout'){
			steps{
				git branch:'master',url:'https://github.com/SameekshaPrabha06/samgrad.git'
			}
		}
		stage('build'){
			steps{
				sh 'gradle build'
			}
		}
		stage('test'){
			steps{
				sh 'gradle test'
			}
		}
		stage('run'){
			steps{
				sh 'gradle run'
			}
		}
	}
}
			
