sa-vpn-openvpn
==============

[![Build Status](https://travis-ci.org/softasap/sa-vpn-opemvpn.svg?branch=master)](https://travis-ci.org/softasap/sa-vpn-openvpn)


Example of use: check box-example

Possible configuration:
```YAML

```

Simple:

```YAML

vars:
     - my_vpn_users:
        - {
            name: "my_user",
            password: "my_password"
          }

roles:

     - {
         role: "sa-vpn-openvpn",
         openvpn_vpn_users: "{{my_vpn_users}}"
       }

```


Advanced:

```YAML

vars:
     - my_vpn_users:
        - {
            name: "my_user",
            password: "my_password"
          }


roles:
     - {
         role: "sa-vpn-openvpn",
         openvpn_vpn_users: "{{my_vpn_users}}"
       }

```



Copyright and license
---------------------

Copyright - Vyacheslav Voronenko

Code licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) or the [MIT License] (http://opensource.org/licenses/MIT).

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)
