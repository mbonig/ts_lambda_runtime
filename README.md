### Typescript Lambda Runtime   

This project builds you a Typescript [runtime for AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html).  With this you can write your Lambda handlers in Typescript without needing to transpile your code first.

See [here]() for more information.

### Building the Runtime

```bash
$ cd src
$ ./build.sh
```

**Note** This currently uses a Node 10.15.1 runtime as the actual executable. Modify your `build.sh` script as you see fit.

Once complete you will have a 'layer.zip' you can upload to your Lambda account. Please refer to these [AWS docs](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html) for information on how.

### Support

I'm offering no direct support, but if you would like to provide feedback, please [create an Issue](https://github.com/mbonig/ts_lambda_runtime/issues/new).
