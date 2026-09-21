# IP Adressing Plan

## IPV4 Addressing

The network uses private IPv4 addressing based on RFC1918 space.

<table align="center">
<th>VLAN
<th>Network
<th>Gateway
<tr>
<td>10
<td>10.10.10.0/24
<td>10.10.10.1
</tr>
<tr>
<td>20
<td>10.10.20.0/24
<td>10.10.20.1
</tr>
<tr>
<td>30
<td>10.10.30.0/24
<td>10.10.30.1
</tr>
<tr>
<td>40
<td>10.10.40.0/24
<td>10.10.40.1
</tr>
<tr>
<td>50
<td>10.10.50.0/24
<td>10.10.50.1
</tr>
<tr>
<td>60
<td>10.10.60.0/24
<td>10.10.60.1
</tr>
<tr>
<td>70
<td>10.10.70.0/24
<td>10.10.70.1
</tr>
<tr>
<td>99
<td>10.10.99.0/24
<td>10.10.99.1
</tr>
</table>

## Addressing Allocation

Suggested allocation:

```text
.1       Gateway
.2-.20   Network infrastructure
.21-.49  Security infrastructure
.50-.99  Servers
.100-.239 DHCP clients
.240-.254 Reserved