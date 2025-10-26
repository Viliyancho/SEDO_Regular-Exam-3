pipeline{
    agent any

    stages{
        stage("Build the application"){
            steps{
                bat 'dotnet build'
            }
        }
        stage("Run the tests"){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
