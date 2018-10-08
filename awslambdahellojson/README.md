# AWS Lambda Function other Hello World Python example

This folder contains an AWS Lambda Function example in Python on AWS (Amazon Web Services).

It handles a simple AWS Lambda function that shows the content (JSON) of the call to the lambda function and returns a message including this content.

## Requirements

* You must have an [Amazon Web Services (AWS)](http://aws.amazon.com/) account.

* The code was written for Python 3.

## Using the code

* Access the AWS console.

* Select AWS Lambda in the services menu.

* Create an AWS lambda function.
  * Name:    <LAMBDA_NAME>
  * Runtime: Python 3.6
  * Role:    lambda-basic-execution
  * The triggers: Nothing
  * The resources the function's role has access: Amazon CloudWatch Logs

  Handler function:

  ```bash
  lambda_function.lambda_handler
  ```

* Write the code.

  The content of `lambda_function.py` file.

* Create and configure a Test event.

  Input file content:

  ```bash
  {
    "firstName": "Peter",
    "lastName": "Parker"
  }
  ```

* Run the code.

  Run the code in an AWS lambda function using the test button.

* Test the AWS Lambda function.

  You should see the next message in the log:

  ```bash
  {
    "message": "Hello Peter Parker!"
  }
  ```