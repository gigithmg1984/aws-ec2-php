pipeline {
    agent any 
    stages {
        stage('AWS Deploy') {
            steps {
                echo 'Hello world!'
                sh 'echo $PWD'
                sh 'scp -i "/home/ubuntu/my-keys.pem" -r aws-ec2-php/* ubuntu@ec2-34-215-51-181.us-west-2.compute.amazonaws.com:/var/www/html'
            }
        }
    }
}
