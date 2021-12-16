node{
    stage('pulling code from github'){
        
        git credentialsId: '8602e083-e32e-4ce1-a44c-071cd5b06c88', url: 'https://github.com/DevopsPavankumar/Latest-Branch.git'
    }
    stage('build the code using maven'){
        sh 'sudo mvn clean install'
    }

    stage('Pulling the image from docker hub'){
        sh 'sudo docker pull jenkins/jenkins' 
    }
    stage('running docker container'){


        sh 'docker run -itd --name Jenkinspipeline -p 9060:9060 jenkins/jenkins'

    }
}
