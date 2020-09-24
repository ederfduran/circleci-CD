# circleci-CD

Simple Example on how to promote to production using a CDN and S3 storage service.
In `.circleci/config.yml` you will just find two jobs

## create_and_deploy_front_end

This is to deploy your website in S3 , at this point it shall already pass all test and stuff from CI pipeline.

## promote_to_production

This step is to update Cloudfront so it will start pointing to your new deployment.

## NOTE:

Do not forget to update your env variables (clientID and Secret) to be able to run aws commands in your instances.
