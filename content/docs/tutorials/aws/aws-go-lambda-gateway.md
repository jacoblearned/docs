---
title: "AWS Golang Lambda With API Gateway | Go"
h1: "AWS Golang Lambda With API Gateway"
linktitle: "AWS Golang Lambda With API Gateway"
no_edit_this_page: true
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/mktutorial. -->

<p class="mb-4 flex">
    <a class="flex flex-wrap items-center rounded text-xs text-white bg-blue-600 border-2 border-blue-600 px-2 mr-2 whitespace-no-wrap hover:text-white" style="height: 32px" href="https://github.com/pulumi/examples/tree/master/aws-go-lambda-gateway" target="_blank">
        <span><i class="fab fa-github pr-2"></i> View Code</span>
    </a>

</p>


This example creates a lambda that does a simple `ToUpper` on the path input of an API request and returns it.

## Deploying the App

To deploy your infrastructure, follow the below steps.

### Prerequisites

1. [Install Pulumi](https://www.pulumi.com/docs/get-started/install/)
2. [Configure AWS Credentials](https://www.pulumi.com/docs/intro/cloud-providers/aws/setup/)
3. [Clone aws-go-lambda](https://github.com/aws/aws-lambda-go)

### Steps

After cloning this repo, run these commands from the working directory:

1. Build the handler:

	- For developers on Linux and macOS:

		```bash
		make build
		```
		
	- For developers on Windows:
		
		- Get the `build-lambda-zip` tool:
			
			```bash
			set GO111MODULE=on
			go.exe get -u github.com/aws/aws-lambda-go/cmd/build-lambda-zip
			```
		
		- Use the tool from your GOPATH:
				
			```bash
			set GOOS=linux
			set GOARCH=amd64
			set CGO_ENABLED=0
			go build -o handler\handler handler\handler.go
			%USERPROFILE%\Go\bin\build-lambda-zip.exe -o handler\handler.zip handler\handler
			```
		

2. Create a new Pulumi stack, which is an isolated deployment target for this example:

	```bash
	pulumi stack init
	```

3. Set the required configuration variables for this program:
	```bash
	$ pulumi config set aws:region us-west-2
	```

4. Execute the Pulumi program to create our lambda:

	```bash
	$ pulumi up                              
	Previewing update (dev):
		Type                           Name               Plan       
	+   pulumi:pulumi:Stack            go-lambda-dev      create     
	+   ├─ aws:apigateway:RestApi      UpperCaseGateway   create     
	+   ├─ aws:iam:Role                task-exec-role     create     
	+   ├─ aws:apigateway:Resource     UpperAPI           create     
	+   ├─ aws:iam:RolePolicy          lambda-log-policy  create     
	+   ├─ aws:apigateway:Method       AnyMethod          create     
	+   ├─ aws:lambda:Function         basicLambda        create     
	+   ├─ aws:lambda:Permission       APIPermission      create     
	+   ├─ aws:apigateway:Integration  LambdaIntegration  create     
	+   └─ aws:apigateway:Deployment   APIDeployment      create     
	
	Resources:
		+ 10 to create

	Do you want to perform this update? yes
	Updating (dev):
		Type                           Name               Status      
	+   pulumi:pulumi:Stack            go-lambda-dev      created     
	+   ├─ aws:apigateway:RestApi      UpperCaseGateway   created     
	+   ├─ aws:iam:Role                task-exec-role     created     
	+   ├─ aws:apigateway:Resource     UpperAPI           created     
	+   ├─ aws:iam:RolePolicy          lambda-log-policy  created     
	+   ├─ aws:apigateway:Method       AnyMethod          created     
	+   ├─ aws:lambda:Function         basicLambda        created     
	+   ├─ aws:apigateway:Integration  LambdaIntegration  created     
	+   ├─ aws:lambda:Permission       APIPermission      created     
	+   └─ aws:apigateway:Deployment   APIDeployment      created     
	
	Outputs:
		invocation URL: "https://<gateway-id>.execute-api.us-west-2.amazonaws.com/prod/{message}"
		lambda        : "arn:aws:lambda:us-west-2:ACCOUNTID:function:basicLambda-75711af"

	Resources:
		+ 10 created

	Duration: 29s
	```

5. Call our lambda function from the cli:

	```bash
	curl https://<gateway-id>.execute-api.us-west-2.amazonaws.com/prod/helloworld   
	HELLOWORLD% 
	```

6. From there, feel free to experiment. Simply making edits, rebuilding your handler, and running `pulumi up` will update your lambda.

7. Afterwards, destroy your stack and remove it:

	```bash
	pulumi destroy --yes
	pulumi stack rm --yes
	```
