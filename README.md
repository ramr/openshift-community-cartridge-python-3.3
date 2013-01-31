OpenShift Community Python 3.3 Cartridge
========================================

This git repository is a community supported cartridge to help you get
started with using Python 3.3.0 on Red Hat's OpenShift PaaS.


Steps to create a Python 3.3 app on OpenShift
---------------------------------------------

Create an account at http://openshift.redhat.com/

Create a namespace, if you haven't already do so

    rhc domain create -n <yournamespace>

Create a python-3.3 application (you can name it anything via -a)

    rhc app create meatpie python-3.3



ssh/virtualenv Caveats
----------------------
When you ssh into your app/gear, you will need to source in a script to setup the library paths and activate the virtual env python 3.3 is installed under.

    ssh  $guid@$app-$ns.rhcloud.com
    rhcsh> source python-3.3/activate_virtenv

.    
.    
... And last but not least, enjoy your flight ... http://xkcd.com/353/


