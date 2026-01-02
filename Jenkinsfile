pipeline {
    agent { label 'worker1' }

    stages { //collection of jobs
        stage ('Run the docker container'){ //job6
        steps{  
            sh 'docker rm -f webos'
            sh 'docker pull rajeshkv10/sampleappdevops40'
            sh 'docker run -dit --name webos -p 90:5000 rajeshkv10/sampleappdevops40'
        }
        }
        
    }
}
