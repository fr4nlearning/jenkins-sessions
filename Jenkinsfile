pipeline{
    agent any

    environment{
        DEMO=1.3
    }

    stages{
        stage('stage-1'){

            echo "This is a build number $BUILD_NUMBER of $DEMO"

            sh '''
                echo "Using a multi shell steps"
                chmod +x test.sh
                ./test.sh
            '''
        }
    }
}