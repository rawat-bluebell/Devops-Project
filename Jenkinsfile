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
       steps
        {
            script{
                 if { expression { params.RELEASE}}   
                    {
                        echo "Publish RELEASE is TRUE."
                    }
                 else 
                    {
                        echo "Publish RELEASE False"   
                    }
                  }
        }
      }
           }
}
