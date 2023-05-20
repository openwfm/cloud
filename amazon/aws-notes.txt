setup command line and python access:

aws.amazon.com -> search IAM -> Users -> add user, groups power user 
click on user -> security credentials tab -> create access key -> local code -> download cvs file to ~.aws
mkdir .aws; chmod 700 .aws
create file ~/.aws/credentials with this: 
[default]
aws_access_key_id = YOUR_ACCESS_KEY
aws_secret_access_key = YOUR_SECRET_KEY
# The following is optional
#aws_session_token = YOUR_SESSION_TOKEN
conda create -n aws awscli boto3
test: 
aws s3 ls



