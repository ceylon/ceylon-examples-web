#Ceylon example on OpenShift

*NB: these instructions are for OpenShift v3. If you want to know about running things on the legacy OpenShift v2 take a look here: [openshift.cartridge](https://github.com/ceylon/openshift-cartridge)*

To run this project on OpenShift v3 you can either use the Web interface or create the application from the command line.

## Web interface

In the web interface after logging in and creating a project you have to click the "Add to Project" button. If "Ceylon" appears in the following list of templates you can select it, if not you must click the "Import YAML/JSON" tab, paste the contents of [this file]() in the text field and click "Create". After this you probably have to click the "Add to Project" button again.

In the following screen you give your application a name and paste the URL to this project: [https://github.com/ceylon-docker/ceylon-example.git#1.3.0](https://github.com/ceylon-docker/ceylon-example.git#1.3.0) in the "Git Repository URL" field.

Now click "Create" and wait. OpenShift will do its work and if everything is okay your application will be ready in a couple of minutes.
 
## Command line

Using the command line you'll first have to log in (the easiest way is to copy it from the OpenShift help option), create a project for it and finally create the application using Ceylon¡s S2I builder:


```shell
$ oc login ....
$ oc new-project <your project name here>
$ oc new-app ceylon/s2i-ceylon:1.3.0~https://github.com/ceylon-docker/ceylon-example.git#1.3.0
```

Now just wait. OpenShift will do its work and if everything is okay your application will be ready in a couple of minutes.
