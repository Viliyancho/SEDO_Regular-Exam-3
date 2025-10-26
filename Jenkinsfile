pipeline{
    agent any

    stages{
        stage("Build the application"){
            when { branch 'main' }
            steps{
                bat 'dotnet build'
            }
        }
        stage("Run the tests"){
            when { branch 'main' }
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
