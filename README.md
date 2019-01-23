ansible-aci-vrf
===============

Manage contexts or VRFs on Cisco ACI fabrics. Each context is a private network associated to a tenant, i.e. VRF.

Requirements
------------

None

Role Variables
--------------

Use the `ansible-doc` module for variables defined by the following modules: 
```
  aci_vrf
```
Use the APIC Object Store Browser http://*APIC-ManagementIP*/visore.html and filter on the following classes:
```
  fvCtx
```
APIC Management Information Model Reference is available at https://developer.cisco.com/docs/apic-mim-ref/.

Dependencies
------------

None

Example Playbook
----------------

```yaml
    - name: Configure ACI
      hosts: APIC
      connection: local
      gather_facts: no

      roles:
        - ansible-aci-include-data
        - ansible-aci-credentials  
        - ansible-aci-tenant  
        - ansible-aci-vrf
```

License
-------

This solution is Copyright (c) 2019 World Wide Technology. All rights reserved. A copy of the applicable end user license agreement for this solution can be obtained by emailing AutomationTeam@wwt.com.

Author Information
------------------

joel.king@wwt.com
