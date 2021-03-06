# Retrieving AWS CloudHSM Client Logs<a name="hsm-client-logs"></a>

You can retrieve the logs generated by the AWS CloudHSM Client\. These logs contain detailed information from the AWS CloudHSM Client daemon\. The location of the logs depends on the operating system of the Amazon EC2 client instance where you run the AWS CloudHSM Client\.

------
#### [ Amazon Linux ]

On Amazon Linux, the AWS CloudHSM Client logs are written to the file named `/opt/cloudhsm/run/cloudhsm_client.log`\. You can use *logrorate* or a similar tool to rotate and manage these logs\.

------
#### [ Amazon Linux 2 ]

On Amazon Linux 2, the AWS CloudHSM Client logs are collected and stored in the *journal*\. You can use *journalctl* to view and manage these logs\. For example, use the following command to view the AWS CloudHSM Client logs\.

```
journalctl -f -u cloudhsm-client
```

------
#### [ CentOS 6 ]

On CentOS 6, the AWS CloudHSM Client logs are written to the file named `/opt/cloudhsm/run/cloudhsm_client.log`\. You can use *logrorate* or a similar tool to rotate and manage these logs\.

------
#### [ CentOS 7 ]

On CentOS 7, the AWS CloudHSM Client logs are collected and stored in the *journal*\. You can use *journalctl* to view and manage these logs\. For example, use the following command to view the AWS CloudHSM Client logs\.

```
journalctl -f -u cloudhsm-client
```

------
#### [ RHEL 6 ]

On Red Hat Enterprise Linux 6, the AWS CloudHSM Client logs are written to the file named `/opt/cloudhsm/run/cloudhsm_client.log`\. You can use *logrorate* or a similar tool to rotate and manage these logs\.

------
#### [ RHEL 7 ]

On Red Hat Enterprise Linux 7, the AWS CloudHSM Client logs are collected and stored in the *journal*\. You can use *journalctl* to view and manage these logs\. For example, use the following command to view the AWS CloudHSM Client logs\.

```
journalctl -f -u cloudhsm-client
```

------
#### [ Ubuntu 16\.04 ]

On Ubuntu, the AWS CloudHSM Client logs are collected and stored in the *journal*\. You can use *journalctl* to view and manage these logs\. For example, use the following command to view the AWS CloudHSM Client logs\.

```
journalctl -f -u cloudhsm-client
```

------
#### [ Windows Server ]

On Microsoft Windows Server, the AWS CloudHSM Client logs are not written to a file\. The logs are displayed in the Command prompt or PowerShell window where you started the AWS CloudHSM Client\.

------