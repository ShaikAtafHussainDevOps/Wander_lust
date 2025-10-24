pipeline{
    agent any
    stages{
        stage("Clone Code from GitHub"){
            steps{
                git url: "https://github.com/ShaikAtafHussainDevOps/Wander_lust.git", branch: "main"
            }
        }
        stage("Deploy using docker-compose"){
            steps{
                sh "docker-compose down -v || true"
                sh "docker-compose up -d"
            }
        }
        stage("deploy"){
            steps{
                echo "this awesome"
            }
        }
    }
}
