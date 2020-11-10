                                 Adding Data To Source

To undertand more  about the data, we may get it from windows to splunk environment in order to do more analysis.

The universal Forwarder helps us gather data from any Windows server by installing it on the host where we want to gather the data from.
Universal forwarders use limited resources. In some cases, such as Registry monitoring, you must use a forwarder, because you cannot collect Registry data over WMI.

                              Splunk forwarders versus WMI. 

If you want to monitor remote Windows data, you may need to use universal forwarder to get data in from a remote Windows host. A universal forwarder offers the most types of data sources, provides more detailed data (for example, in performance monitoring metrics), minimizes network overhead, and reduces operational risk and complexity. It is also more scalable than WMI in many cases. WMI rarely works with Splunk apps and solutions, including Splunk premium apps. Finally, due to the security concerns, forwarder is much more recommended than WMI.

In choosing the user Splunk Enterprise should run as, the user determines what Splunk Enterprise can monitor. And for installation options, the Splunk Universal Forwarder documentation has many topics related to installation on Windows. A best practice is to perform the installation a consistent way with limited post installation configuration. 

