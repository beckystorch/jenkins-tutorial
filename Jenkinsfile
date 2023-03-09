pipeline{
        agent any
        stages{
            stage('Clone repo'){
                steps{
                    sh "git clone https://gitlab.com/qacdevops/chaperootodo_client"
                }
            }
            stage('Deploy app'){
                steps{
                    sh "docker-compose pull && DB_PASSWORD=PASSWORD docker-compose up -d."
                        
                }
            }
        }
}
