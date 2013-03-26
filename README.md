Scripts
=======

While working at University of Wisconsin Milwaukee I made this script.

This script is a workflow selection script for DeployStudio. Essentially it contains every Apple Machine Model name. 
The script pulls the model name and then determines from several arrays what the maximum operating system is
that the machine can run.

Then it will run the workflow that you designate for 10.6, 10.7, and 10.8. This needs to be modified with the correct
workflow keys before it will work.

There is also an if do statement that determines where the machine has been set up by looking for the .applesetupdone file.
If the file isn't there then we assume that the computer is new and already has a fresh OS on it. It then points to a
workflow that installs packages rather than laying down an operating sytem.
