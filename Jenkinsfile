//CODE_CHAGES = getGitchanges --- this is groovy script which will check if there any changes in code-bases

pipeline{
    agent any

    environment {
        NEW_VERSION = '1.3.0'
    }


    stages{
        stage ("build"){
            // when{
            //     expression{
            //         BRANCH_NAME == 'dev' && CODE_CHANGES == true
            //     }
            // }            
            steps {
                echo "buliding the application"
                echo "building version ${NEW_VERSION}"


            }
        }
        stage ("test"){
            // when{
            //     expression{
            //         BRANCH_NAME == 'dev'
            //     }
            // }
            steps {
                echo "buliding the application"
            }
        }
        stage ("deploy"){
            steps {
                echo "buliding the application"
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
