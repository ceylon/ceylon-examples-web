#Ceylon example project

This project contains a demo web application named `ceylon.demo.net` that contains both a server-side part and a client-side part. Both are written in Ceylon but one will be compiled for the JVM backend and act as the server while the other will be compiled to JavaScript for use in the client's browser. The project structure is as follows:

```
- README               # This file
- source/...           # The example's Ceylon source files
- web-content/...      # The example's HTML files, stylesheets, images and 3rd party JS libraries
- .config/...          # The place for Ceylon-specific configuration files
- ceylonb[.bat]        # THe Ceylon bootstrap script for running Ceylon without having it installed
```

## Compiling the project

To compile the project you can run the following command (you can ignore any warnings):

    ./ceylonb compile,compile-js

## Running the project

And to run the project we simply run:

    ./ceylonb run
    
