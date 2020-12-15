# Short Instruction

func init <<PROJECTNAME>> --worker-runtime powershell --docker
cd <<PROJECTNAME>>
func new --name <<FUNCTIONNAME>> --template "HTTP trigger"

az login
az acr build --registry <<REGISTRYNAME>> --image <<IMAGENAME>>:v1.0.0 .