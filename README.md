README
======

Spatial Temporal Oceanographic Query System (STOQS)
---------------------------------------------------

STOQS is a geospatial database and web application designed for providing efficient 
acccess to *in situ* oceanographic data across any dimension.
See http://www.stoqs.org for more information.

Getting started with a STOQS development system with [Vagrant](http://docs.vagrantup.com/v2/installation/index.html)i
and [VirtualBox](https://www.virtualbox.org/wiki/Downloads):

    curl "https://raw.githubusercontent.com/MBARIMike/stoqs/django17upgrade/Vagrantfile" -o Vagrantfile
    curl "https://raw.githubusercontent.com/MBARIMike/stoqs/django17upgrade/provision_centos.sh" -o provision_centos.sh
    vagrant up --provider virtualbox

After your virtual machine has booted log in, finish the Python setup, and load some test data:

    vagrant ssh 
    cd dev/stoqsgit
    source venv-stoqs/bin/activate
    ./setup.sh
    ./load.sh
    ./test.sh

Visit your own server's STOQS User interface:

    http://localhost:8000



The stoqs project web site has a wiki with links to presentations and periodic feature
updates.  The [stoqs-discuss](https://groups.google.com/forum/#!forum/stoqs-discuss) list in Google Groups is also a good place to post questions
or any sort of comments about STOQS.    



