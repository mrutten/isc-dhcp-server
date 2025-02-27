# ISC DHCP server playbook

## Table of Contents

<!--toc:start-->

- [ISC DHCP server playbook](#isc-dhcp-server-playbook)
  - [Table of Contents](#table-of-contents)
  - [Usage](#usage) - [Generate a Secure OMAPI Key](#generate-a-secure-omapi-key)
  <!--toc:end-->

## Usage

Substitute the appropriate values in `inventory/group_vars/dhcpservers.yml`.

### Generate a Secure OMAPI Key

Generate a secure OMAPI key using the command below and paste the resulting value in `inventory/group_vars/dhcpservers.yml` as the `omapi_secret` value.

```bash
sudo tsig-keygen -a HMAC-SHA256 omapi_key
```
