# Debugging Alfresco running in Docker container.

The containers we are building are running Alfresco and Share using the installer. (This might not be how we are doing this in the future.) This means that we can use the alfresco.sh script to start the apps. If you need to get the web apps to run with the a jdwp debugger we can modify the setenv.sh script to include the parameters `-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=8000`. You also need to expose the port specified in the address parameter. In this case `8000`.

We ultimately need a way to configure containers to turn this functionality on and of so that if a developer needs to capture to dig more into the code he doesn't need to be modify working files he can just modify the a config file or pass a command line argument.
