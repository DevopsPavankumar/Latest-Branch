node{
    stage('i am pulling code from github'){
        git credentialsId: 'd1bba3c0-a041-495f-9837-db4600aa15bb', url: 'https://github.com/DevopsPavankumar/Latest-Branch.git'
    }
    
    stage('build the code using maven'){
        sh 'mvn clean install'
    }
    stage('Pulling the image from docker hub'){
        sh 'sudo docker pull nginx' 

    stage('running docker container'){
        sh 'docker run -itd --name Nginxweb -p 8000:80 nginx'

    }
    
}
