pipeline {
  
  agent any
    
    stages {
        stage('First Stage') {
            steps {
                echo "this is my frist stage"
            }
        }

        stage('First Stage') {
            steps {
                echo "this is my frist stage"
            }
            post {
                success {
                    archiveArtifacts artifacts: '**/spring-petclinic-*.jar'
                    junit testResults: '**/TEST-*.xml'
                    mail subject: 'build stage succeded',
                         from: 'build@learningthoughts.io',
                         to: 'all@learningthoughts.io',
                         body: "Refer to $BUILD_URL for more details"
                }
                failure {
                    mail subject: 'build stage failed',
                         from: 'build@learningthoughts.io',
                         to: 'all@learningthoughts.io',
                         body: "Refer to $BUILD_URL for more details"
                }
            }
        }
    }
}
