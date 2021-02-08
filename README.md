# aws-amplify-react-github-action
Template for deploying a Create React App (CRA) to AWS Amplify

## Getting Started

1. Copy this file into `.github/actions` on the root of your project.
2. Follow the AWS User Account settings documentation here: 
    * https://github.com/marketplace/actions/amplify-cli-action#configuration
    * https://github.com/marketplace/actions/amplify-cli-action#aws-credentials-controlling-access-with-iam
3. At this point, you should have two GitHub secrets: `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`.

> If you already have hosting setup with AWS Amplify, then it will bypass GitHub actions.  I recommend setting up an S3 and Cloudfront hosting by following this link: https://docs.amplify.aws/cli/hosting#amazon-s3-and-amazon-cloudfront

4. Adjust any branch and PR triggers on lines 2-6.
5. Adjust your supported `node-version`s on line 14. (Some people have to support different versions, so I accounted for that here)
6. On lines 35, 38, and 41, you'll need to have the appropriate scripts in place so see `package.json` as an example.
