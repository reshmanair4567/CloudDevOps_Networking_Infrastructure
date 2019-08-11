Used Luchidchart to design and implement cloud architecture diagram for a web application architecture on AWS. 
Created multi-AZs within a VPC , created private and public subnets and internet gatway to filter and control traffic.
Added Routing table rules to the network. 
Implemented Infrastructure as Code using CloudFormation code in YAML.

AWS CLI commands :
To create Infrastructure:
aws cloudformation create-stack --stack-name infrastack --region us-west-2 --template-body file://ourinfra.yml --parameters ourinfra-params.json
or use the better approach -
./create.sh infrastack ourinfra.yml ourinfra-params.json

Similarly , To update infrastructure:
./update.sh infrastack ourinfra.yml ourinfra-params.json

