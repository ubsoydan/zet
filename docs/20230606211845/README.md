# Changes in SSH fingerprint

You wouldn't expect to see any change in ssh fingerprint when you are dealing with VMs, right? But that's not the case. Apparently, any change with the IP address registered in the fingerprint ends up changing fingerprint as well. So, it may not necessarily mean you have been hacked or compromised somehow. Make sure you are connecting from the same PC which you made first SSH connection with.


If you can't still SSH into the machine for some reason, open up the direct console of that machine and then modify known_hosts folder that contains fingerprint records so that you can make it ask for a new fingerprint. Can be troublesome, but it's all for security.
