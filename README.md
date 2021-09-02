# ADF-Functions

## Deploy to Azure
[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Foh22is%2FADF-Functions%2Fmain%2FmainTemplate.json)  [![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](https://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Foh22is%2FADF-Functions%2Fmain%2FmainTemplate.json)

## Resources

The resources are created to be used as functions in ADF or Synapse.

| ResourceType                         | DeploymentName | DependsOn | Language |
|-----------------------------------------|----------------|-----------|-----------|
| pid-0d687f89-584c-4ea6-a25e-436b2c363671 | same like resource type | none      | none|  
| App Service Plan                         | deploy_plan    | none      |  none |
| Function App, Storage Account, Application Insights | deploy_func_dynamics365 | deploy_plan |  |
| Function App, Storage Account, Application Insights | deploy_func_hashgeneration | deploy_plan |   |
| Function App, Storage Account, Application Insights | deploy_func_notifications | deploy_plan |   |
| Function App, Storage Account, Application Insights | deploy_func_profiling | deploy_plan |  | 
| Function App, Storage Account, Application Insights | deploy_func_filemerge | deploy_plan | |
| Function App, Storage Account, Application Insights | deploy_func_deploybranchtoadf | deploy_plan | | 
| Function App, Storage Account, Application Insights | deploy_func_synapsebuilder | deploy_plan |  |
| Function App, Storage Account, Application Insights | deploy_func_synapsebuilderutilities | deploy_plan |   | 
| Function App, Storage Account, Application Insights | deploy_func_executepipeline | deploy_plan |   dotnet |

## What's next?
At this point you have the underlying resources avaiable.

Time to deploy the code, create a service principal for the functions and assign the permissions 

For further steps or help, please check our deployment guide.
