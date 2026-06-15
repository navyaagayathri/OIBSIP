## Objective
Perform a network scan to identify open ports and services running on a local machine using Nmap.

## Tools Used
- Nmap

## Procedure
1. Installed Nmap on the system.
2. Performed a scan on the local machine using the command below.
3. Reviewed the scan output to identify open ports and the services running on them.
4. Documented the results for analysis.

## Scan Command Used
```bash
nmap localhost
```

## Scan Results

| Port | Service | Description |
|------|---------|-------------|
| 135 | MSRPC | Used by Windows for remote procedure calls between applications. |
| 445 | Microsoft-DS | SMB service, used for file and printer sharing on a network. |

## Findings
The scan found two open ports on the local machine - port 135 (MSRPC) and port 445 (Microsoft-DS). Both are default services on Windows systems, used mainly for internal communication and file sharing. These ports are also commonly mentioned in security discussions since older SMB versions have known vulnerabilities, so keeping them updated and firewalled is generally recommended.

## Result
The scan was completed successfully and the open ports/services on the local machine were identified.

## Conclusion
This task helped in understanding how Nmap can be used for basic network scanning - identifying live hosts, open ports, and the services tied to them. It's a useful first step in learning how network reconnaissance works in practice.

