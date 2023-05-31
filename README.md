# cloudformation-tinyproxy

A cloudformation template to deploy tinyproxy containers into ECS and proxy your traffic through the AWS Public IP Range

## Instructions:
1. Navigate to AWS Console -> Cloudformation -> Create Stack
2. Upload cfn-tinyproxy.yaml
3. Select required parameters
4. Wait for stack to deploy
5. ```curl --proxy <aws_ip>:8888 <https://your_endpoint.com>``` - your traffic will be proxied through the AWS Public iP
6. Stop and Start the container if you need a new IP
7. To tear down resources immediately, simply go to Cloudformation console and delete stack

Full writeup @ https://vvinoth.com/post/tinyproxy
