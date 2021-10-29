# Develop with Okteto, NGINX, and PHP-FPM

[![Develop on Okteto](https://okteto.com/develop-okteto.svg)](https://github.com/okteto/php-with-nginx)

This sample will show you how to develop an NGINX + PHP-FPM application directly in Kubernetes with Okteto.

1.  Deploy your Kubernetes application by either clicking on the green button (if using Okteto Cloud) or using the Kubernetes manifests in the `manifests` folder.

1. Once your application is up and running, try it out. Open your browser and access the index.php file. You'll see something like this:

```
Hello PHP
```

1. Now, let's develop directly in the cluster. First, activate your development environment by running the following commands:
```
$ cd app
$ okteto up
```

> If this is the first you use Okteto, you'll need to [install the okteto CLI](https://okteto.com/docs/getting-started/installation/). 

1. As long as `okteto up` is running, your local file system is connected to your remote development environment. Any change on the application code will be automatically synchronized and applied in your remote development environment. 

1. Now try it out. Open the [index.php](app/index.php) file and change the string to "Hello from my remote development environment". Save the file, open your browser, and access the PHP file.

```
Hello from my remote development environment
```

This repository is an example to show you how you can use okteto to develop directly in your remote development environment. While the application is simple, we hope it gives you a good overview of the power of remote development. Check out our [samples repository](https://github.com/okteto/samples) to continue to learn more about the power of Okteto.

