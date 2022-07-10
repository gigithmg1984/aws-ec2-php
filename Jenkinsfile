pipeline {
    agent any 
    stages {
        stage('AWS Deploy') {
            steps {
                echo 'Hello world!'
                sh 'echo $PWD'
                sh 'scp -i "/jenkins/my-keys.pem" -r /tmp/projects/aws-ec2-php/* ubuntu@ec2-34-215-51-181.us-west-2.compute.amazonaws.com:/var/www/html'
            }
        }
    }
}
