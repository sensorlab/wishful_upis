Wishful Upi packages
====================

There are in total 2 major categories of UPIs, namely the UPI_R (physical and MAC layer control) and the UPI_N (network layer control). The implemented framework offers the possibility to execute the supported UPI_R and UPI_N from a global controller through the use of UPI_G or from a local controller through the usage of UPI_L. Also a hierarchical interface for the exchange of messages between local and global control programs.

.. automodule:: wishful_upis
    :members:
    :undoc-members:
    :show-inheritance:

Submodules
----------

UPI_M: Management interface
---------------------------

The UPI_M is used to enable the use of a specific execution enviroment in a node and also for the initialization of nodes before starting an experiment. MAC protocol update will also be supported in the next version of the interface based on the supported MAC engines.

The WISHFUL interface definitions - UPIs (UPI_M) for install/update/active/deactive software modules.

.. automodule:: wishful_upis.mgmt
    :members:
    :undoc-members:
    :show-inheritance:

UPI_N: Network layer programming interfaces
-------------------------------------------

        Unified Programming Interface – Network(UPI_N) : this is a software interface consisting of a set of functions that ensures uniform control of the upper MAC and network layer protocol behavior on heterogeneous devices. The functions forming the interface are generic, their implementation is hardware and platform specific and is provided by the Local Monitoring and Configuration engine. The user is able to manipulate a wide range of network layer fucntionality like routing, flow control, queue management, priority control and more.



.. automodule:: wishful_upis.net
    :members:
    :undoc-members:
    :show-inheritance:

UPI_R: Radio layer programming interfaces
-----------------------------------------

        Unified Programming Interface – Radio (UPI_R) : this is a software interface consisting of a set of functions that ensures uniform control of the radio and lower MAC behaviour on heterogeneous devices. The functions forming the interface are generic, their implementation is hardware and platform specific and is provided by the Local Monitoring and Configuration engine. Monitoring of parameters, taking measurements at any time and total control of all exposed parameters of the afforementioned layers is made possible through UPI_R for all supported platforms, providing unprecented flexibility of control on the targeted platforms.

.. automodule:: wishful_upis.radio
    :members:
    :undoc-members:
    :show-inheritance:

"Network OS" helpers
--------------------

The functions supported offer a kind of "Network OS" functionality making it easy for the user to get network wide information regarding communication and interference range for all nodes in the network as well as link parameters for all links present. These helpers are of course based on the basic UPIs offered from UPI_N and UPI_R.

.. automodule:: wishful_upis.net_func
    :members:
    :undoc-members:
    :show-inheritance:

Subpackages
-----------

.. toctree::

    wishful_upis.lowpan
    wishful_upis.lte
    wishful_upis.wifi



