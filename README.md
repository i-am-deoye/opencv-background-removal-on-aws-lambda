# OpenCV Background Removal On AWS Lambda

Serverless removal of images backgrounds with OpenCV, using an AWS Lambda.

# How to Use

1. Click the "OpenCV Object Detection Launch Stack" button:

[![OpenCV Background Removal Launch Stack](read-me-images/ImageBackgroundRemovalLaunchStack.png)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=OpenCVObjectDetectionStack&templateURL=https://opencv-source.s3.amazonaws.com/template.yaml)


This will bring you to either the Cloudformation UI or the AWS console if you are not signed in. Sign in, if you are not already. From the Cloudformation UI, click "Next" at the bottom of the screen. Repeat clicking "Next" on the two following pages. You will reach a page with this towards the bottom:

![CloudFormation Shot](/read-me-images/CloudFormationShot.png?raw=true)

&nbsp;

Checkmark the three "I acknowledgement" statements and select "Create Stack." This will start building the CloudFormation stack.

&nbsp;

2) Navigate to S3. You should see a bucket named "opencv-demo-xxxxxxxx", where "xxxxxxxx" is the unique stack identifier from CloudFormation. Open this bucket. You will see an "index.html" file. Open this file. This webpage will appear:

![OpenCV Object Detection Screen Shot](read-me-images/OpenCVScreenShot.png?raw=true)

&nbsp;

If you select the "Object Detections Options" or "Haar Cascade Face Detection Options", you can control which object detection models or Haar Cascade models you use. The "Output Visualization Options" allows you to control the output image appearance and set a minimum confidence threshold for the AWS Rekognition and OpenCV DNN models. The minimum confidence threshold for the Haar Cascade models is 50%.

![OpenCV Object Detection Menu Screen Shot](read-me-images/OpenCVMenuShot.png?raw=true)

&nbsp;

3) Select a photo. Either select one of the stock photos or upload your own image. Select "Detect," if you uploaded an image or changed the image detection options.

![OpenCV Detection Menu Screen Shot](read-me-images/OpenCVDetectionShot.png?raw=true)

&nbsp;

4) Congratulations! It's that easy.

&nbsp;

# Questions

Any questions or suggestions, just add an "Issues" submission to this repository. Thanks.

&nbsp;

Happy Coding!

