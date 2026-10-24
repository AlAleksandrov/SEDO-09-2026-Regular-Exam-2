pipeline{
    agent any
    stages{
        stage("Restore dependencies"){
            steps{
                 bat "dotnet restore" // Restore dependencies for Windows machines
            }
        }
        stage("Build the project"){
            steps{
                 bat "dotnet build --no-restore" // Build the project for Windows machines
            }
        }
        stage("Run tests"){
            steps{
                 bat "dotnet test --no-build --verbosity normal" // Run tests for Windows machines
            }
        }
    }
}
