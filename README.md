# serverless-goof
A sample vulnerable serverless application

# a way to deploy
0. Ensure you have an AWS account, Lambda, and the AWS CLI installed and configured
1. Create a "serverless-goof" function in Lambda
2. Clone this repo to a local working directory
3. Run "npm install" or "npm ci" and this will install the modules into node_modules and provide a package-lock.json
4. Zip it with "zip -r serverless-goof.zip ."
5. Upload it: "aws lambda update-function-code --function-name serverless-goof --zip-file \  "fileb:///Users/youraccount/workingdir/serverless-goof.zip"
