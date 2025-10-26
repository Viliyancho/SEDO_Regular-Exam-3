pipeline{
    agent any

    stages{
        stage("Build the application"){
            when { branch pattern: "main", comparator: "REGEXP" }
            steps{
                bat 'dotnet build'
            }
        }
        stage("Run the tests"){
            when { branch pattern: "main", comparator: "REGEXP" }
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
