deployr-rserve
==============

`deployr-rserve` is a fork of the popular R package, [Rserve](https://github.com/s-u/Rserve) from Simon Urbanek.  
This fork adds the following features:

1.  Concurrent R sessions under Rserve on the Windows platform
2. Ability to switch the execution context of the Rserve process to a specified uid/gid
3. Out-of-band control socket that supports a cancel operation on any Rserve eval operation

This fork is based on Rserve `0.6-3.1`.

Installations of DeployR require `deployr-rserve`.  The standard [Rserve](https://github.com/s-u/Rserve) package does not include the necessary functionality to work with [DeployR](https://github.com/deployr/server).
