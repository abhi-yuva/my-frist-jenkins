pipeline {
     agent{
        label 'slave'
    }
    
    parameters {
        choice choices: ['dev','stage','prod'], description: 'My Environments', name: 'env'
    }
    stages{
        stage ('Build') {
            steps{
                script{
                    // this is for dev environment
                    if (params.env == 'dev'){
                        echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'stage'){
                          echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'prod'){
                         echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }
                }
            }
        }

        stage ('Package') {
            steps{
                script{
                    // this is for dev environment
                    if (params.env == 'dev'){
                        echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'stage'){
                          echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'prod'){
                         echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"


                    }
                }
            }
        }

        stage ('deploy') {
            steps{
                script{
                    // this is for dev environment
                   if (params.env == 'dev'){
                        echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'stage'){
                          echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }

                    if (params.env == 'prod'){
                         echo " This is my ${params.env} Environmet"
                        echo "I am running in ${params.env} Evnironment"

                    }
                }
            }
        }
    }
    post {
        success{
            script{
                echo "My ${params.env} Build Was Sucess"
            }
        }

        failure{
            script{
                echo "My ${params.env} Build Was Failed"
            }
        }
    }
}
