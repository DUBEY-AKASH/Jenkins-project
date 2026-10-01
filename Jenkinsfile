//CODE_CHAGES = getGitchanges --- this is groovy script which will check if there any changes in code-bases

pipeline{
    agent any

    parameters{
        string(name: 'version', defaultValue: '', description: 'version to deploy on prod')
        choice(name: 'version', choices:['1.1.0', '1.2.0'], description:'')
        booleanParam(name: 'excuteTests', defaultValue: true, description: '')
    }

    // tools{
    //     maven 'Maven'   ------- Use of tools
    // }

    // environment {
    //     NEW_VERSION = '1.3.0'
    //     SERVER_CREDENTIALS = credentials('CRED_MB_GH')  ---- example of declaring environment variables
    // }


    stages{
        stage ("build"){
            // when{
            //     expression{
            //         BRANCH_NAME == 'dev' && CODE_CHANGES == true
            //     }
            // }            
            steps {
                echo "buliding the application"
                // echo "building version ${NEW_VERSION}"


            }
        }
        stage ("test"){
            when{
                expression{
                    params.excuteTests == true
                }
            }
            steps {
                echo "buliding the application"
            }
        }
        stage ("deploy"){
            steps {
                echo "buliding the application"
                // echo "deploying with ${SERVER_CREDENTIALS}"
                // sh "SERVER_CREDENTIALS" /// another way of using credentials is withCredentials

                // withCredentials([
                //     usernamePassword(credentials: 'CRED_MB_GH', usernameVariable: USER, passwordVariable: PWD)
                // ]){
                //     sh "Script ${USER} ${PWD}"
                // }

                echo "deploying version ${params.VERSION}"
            }
        }
    }

    // post{
    //     always {
    //         //if the pipeline fails or suceeds whatever happens post attribute will always run

            
    //     }
    //     success{

    //     }

    //     failure{

    //     }
    // }
}
