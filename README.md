# Short Instruction

https://docs.microsoft.com/en-us/azure/azure-functions/functions-create-function-linux-custom-image?tabs=bash%2Cportal&pivots=programming-language-powershell

func init PROJECTNAME --worker-runtime powershell --docker
cd PROJECTNAME
func new --name FUNCTIONNAME --template "HTTP trigger"

az login
az acr build --registry REGISTRYNAME --image IMAGENAME:v1.0.0 .



// Change AuthLevel in function.json to anonymous
