# Data migration from ARCHER to ARCHER2

## Log on to ARCHER

[Log on to ARCHER](http://www.archer.ac.uk/documentation/user-guide/connecting.php#sec-2.1) as usual

## Load up-to-date version of ssh on Archer
 
    module load ssh


## scp your file

Use a less heavyweight encryption cypher, e.g., via option

    scp -c aes128-gcm@openssh.com <file> user@transfer.dyn.archer2.ac.uk:<path>

(Remember to replace **user** with your ARCHER2 username in the example above.)

Use the address **transfer.dyn.archer2.ac.uk** in preference to login.archer2.ac.uk. The former provides a route with a higher peak bandwidth. The same ssh key pair can be used for either.

For full details of Archer to Archer2 transfers, please see  the [ssh data transfer example](../data#ssh-data-transfer-example).

