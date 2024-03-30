pipeline {
  
  agent any
    
    stages {
        stage('First Stage') {
            steps {
                echo "this is my frist stage"
            }
        }

        stage('second Stage') {
            steps {
                echo "this is my frist stage"
            }
            post {
                success {
                    mail subject: 'build stage failed',
                         from: 'devopsbyabhi@gmail.com',
                         to: 'devopsbyabhi@gmail.com',
                         body: "Refer to $BUILD_URL for more details"
                }
            }
        }
    }
}
