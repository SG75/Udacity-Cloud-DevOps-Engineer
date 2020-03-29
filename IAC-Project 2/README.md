Project Name: Udagram 
	       Deploy a high-availability web app using CloudFormation
Course: Udacity Cloud DevOps NanoDegree
Files:
    
    1. Udagram-parameters-server.json -- Parameters file for Server Infrastructure 
    2. Udagram-servers.yaml           -- cloudformation YAML script to create stack for Server Infrastructure
    3. Udagram-parameters.json        -- Parameters file for Network Infrastructure 
    4. Udagram-servers.yaml           -- cloudformation YAML Script to create stack for Network Infrastructure 
    5. create-udagram-net.bat	      -- batch file to create network infrastructure stack
    6. create-udagram-servers.bat     -- batch file to create servers infrastructure stack
    7. delete-udagram-net.bat	      -- batch file to delete network infrastructure stack
    8. delete-udagram-servers.bat     -- batch file to delete servers infrastructure stack
    9. udagram.pdg		              -- Pictorial representation of udagram infrastructure


By default these .bat files uses "us-west-2" as region for stack creation
to create a stack in another region, edit the region in the .bat file

Example Syntax: 
```
aws cloudformation <create|update|delete> --stack-name <name for the stack> 
                            --template-body file://<.yaml> 
                            --parameters file://<.json>
                            --region=<region> 
                            --capabilities CAPABILITY_IAM
```
                

