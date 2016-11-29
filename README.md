#Ceylon example project

This project contains a demo web application named `ceylon.demo.net` that contains both a server-side part and a client-side part. Both are written in Ceylon but one will be compiled for the JVM backend and act as the server while the other will be compiled to JavaScript for use in the client's browser. The project structure is as follows:

```
- README               # Useful info
- modules              # The place where the compiled modules will go
- source/...           # Your module source files
- resource/...         # Your module resource files (if any)
- web-content/...      # The default template module's resources, you can remove it if you don't need it
```

## Compiling the project

To compile the project you can run the following command (you can ignore any warnings):

    ./ceylonb compile,compile-js

## Running the project

And to run the project we simply run:

    ./ceylonb run
    
