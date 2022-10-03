pipeline 
{
    agent any

    stages 
    {
        stage('build') 
        {
            steps 
            {
                echo 'build app'
            }
        }
        
        stage('test') 
        {
            steps 
            {
                echo 'test app'
            }
        }
        
        stage('deploy') 
        {
            steps 
            {
                echo 'deploy app'
            }
        }
    }

    post
    {
       always
       {
          emailext body: 'environmental development', subject: 'pipeline status', to: 'vachanapatil112@gmail.com'
       }
    }
}
