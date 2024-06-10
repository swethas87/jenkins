pipeline {
    agent {
        label 'agent1'
    }
      options {
        timeout(time: 1, unit: 'SECONDS')
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                //
                sh 'echo This is build'
            }
        }
        stage('Test') {
            steps {
                //
                sh 'echo This is Test'
                sh'sleep 10'
            }
        }
        stage('Deploy') {
            steps {
                //
                sh 'echo This is Deploy'
            }
        }
    }
}