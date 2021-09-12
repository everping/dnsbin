## Introduction
DNSBin is a tool to test data exfiltration through DNS. It's helpful for testing out of band attacks when testers try to prove that they can execute commands on a targeted server by connecting to a public domain.

## Usage
1. Generate a random string like `iuhwqerojisdf234df`
2. Perform a `ping`, `dig`, `nslookup`, etc to the domain `iuhwqerojisdf234df.test.dnsbin.net`. Note that you have to replace the random string with your string.
3. DNSBin will receive your DNS query and you can check whether it is successful or not by requesting to `https://dnsbin.net/verify/test/iuhwqerojisdf234df`. You get the status true if the command is executed successfully and get false for the failed command.

```shell
    curl https://dnsbin.net/verify/test/iuhwqerojisdf234df

    {"status": true}
```
                                
