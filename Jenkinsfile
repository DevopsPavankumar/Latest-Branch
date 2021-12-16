node{
    stage('i am pulling code from github'){
        git credentialsId: 'd1bba3c0-a041-495f-9837-db4600aa15bb', url: 'https://github.com/DevopsPavankumar/Latest-Branch.git'
    }
    
    stage('build the code using maven'){
        sh 'mvn clean install'
    }

    stage('running docker container'){
        sh 'docker run -itd --name Jenkins -p 9050:9050 jenkins/jenkins'

    }
    
}
