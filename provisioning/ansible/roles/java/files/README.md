There are programmatic solutions out there for accepting Oracle's licensing agreement during a scripted download.
Most of them seem hackish and quite brittle.  So rather than deal with all that licensing mumbo jumbo in a script,
by convention this [Ansible](http://www.ansibleworks.com/) role looks to this directory for its Java binaries.

Copy your downloaded Java rpm's or gz's to this directory.  Be sure to update this role's defaults/main.yml with
the correct version info. Or better yet, update vars/os_defaults.yml or vars/{{ ansible_os_family }}.yml in your
playbook's directory. 

For downloading binaries, go to Oracle's [website](http://www.oracle.com/technetwork/java/javase/downloads/index.html).
