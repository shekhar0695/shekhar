pipeline {
    agent any 
    stages{
        stage('BUILD') {
            steps{
                 sh '''
                    make
                    echo "This is a BUILD stage"
                '''
            }
        }

        stage('TEST') {
            steps{
                sh '''
                    sleep 6
                    echo "This is a TEST stage"
                '''
            }
        }

        stage('DEPLOY') {
            steps{
                sh '''
                    sleep 5
                    echo "This is a DEPLOY stage"
                '''
            }
        }
        stage('POST bUILD') {
            steps{
                sh 'echo "This is a POST BUILD stage"'  
            }
        }   
    }
}
