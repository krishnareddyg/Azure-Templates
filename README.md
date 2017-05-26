# Azure-Templates

This repo contains all currently available Azure Resource Manager templates contributed by the community. A searchable template index is maintained at https://azure.microsoft.com/en-us/documentation/templates/. The following information is relevant to get started with contributing to this repository.

Contribution guide. Describes the minimal guidelines for contributing.
Best practices. Best practices for improving the quality of your template design.
Git tutorial. Step by step to get you started with Git.
Useful Tools. Useful resources and tools for Azure development.
Deploying Samples

You can deploy these samples directly through the Azure Portal or by using the scripts supplied in the root of the repo.

To deploy a sample using the Azure Portal, click the Deploy to Azure button found in the README.md of each sample.

To deploy the sample via the command line (using Azure PowerShell or the Azure CLI 1.0) you can use the scripts below.

Simply execute the script and pass in the folder name of the sample you want to deploy.

For example:

PowerShell

.\Deploy-AzureResourceGroup.ps1 -ResourceGroupLocation 'eastus' -ArtifactStagingDirectory '[foldername]'
Bash

Please ensure that you have node and npm, jq and azure-cli installed.

./azure-group-deploy.sh -a [foldername] -l eastus
If you see the following error: "syntax error near unexpected token `$'in\r''", run this command: 'dos2unix azure-group-deploy.sh'.
If you see the following error: "jq: command not found", run this command: "sudo apt install jq".
If you see the following error: "node: not found", install node and npm.
If you see the following error: "azure-group-deploy.sh is not a command", make sure you run "chmod +x azure-group-deploy.sh".
