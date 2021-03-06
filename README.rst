=======
SDN 101
=======
Introduction
------------
With the advent of SDN, the advancing of the customizable networks has been accelerated.
Its focus is mainly on the control-ability of the programs.
SDN guarantees to significantly ease the network management and
it also brings this opportunity of applying new ideas into current networks immediately.

In this repository you can find some sample codes of SDN written on `ELRYU controller`_ and for more information you can
see documentation section. I wrote all of these introduction and sample codes as my intern project in ITRC_.

Project
-------
As a project we implemented simple firewall with python 3 on `ELRyu controller`_,
and for testing it we used `mininet platform`_.

I personally prefer python3 so I ported `Ryu Controller`_ on python3 and named it `ELRyu Controller`_

Usage's Sample
..............
1. Run firewall application on ryu with following command::

    $ ryu-manager sdn101/app/rest_firewall.py

2. Run mininet with your custom options using command that like following command::

    $ sudo mn --switch=ovs,protocol=OpenFlow13 --controller=remote,x.x.x.x

3. Run firewall client application with following command::

    $ python3 sdn101/firewall_client_cli.py

4. Enter your server ip address and port.
5. Use Firewall CLI Client in order to manage your firewall and have fun :))

Documentation
-------------
A Persian documentation about SDN and it's history can be found in `Introduction to SDN`_ on my google drive.

Contributors
------------
1. `Elahe Jalalpour`_

.. _ELRyu Controller: https://github.com/elahejalalpour/ELRyu
.. _mininet platform: http://mininet.org/
.. _Introduction to SDN: https://docs.google.com/document/d/1ViS_8O3iC8ExZQHhwPMEqcHDuvHJ4gotTIst0r7YYg0/edit?usp=sharing
.. _Ryu controller: https://github.com/osrg/ryu
.. _ITRC: https://www.itrc.ac.ir/
.. _Elahe Jalalpour: http://ceit.aut.ac.ir/~jalalpour
