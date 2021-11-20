pipeline{
    agent any
    parameters
    {
      booleanParam(name: "RELEASE", defaultValue: false)
    }
    stages{
      stage("build")
      {
        steps
        {
          echo "build the code"
        }
      }
      stage("Publish")
      {
       when { expression { params.RELEASE}}   
        steps
        {
          echo "Publish the code"
        }
      }
      
    }
}
