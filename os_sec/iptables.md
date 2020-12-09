# Iptables

__Docs:__

- https://www.digitalocean.com/community/tutorials/iptables-essentials-common-firewall-rules-and-commands#saving-rules
- https://www.digitalocean.com/community/tutorials/how-to-list-and-delete-iptables-firewall-rules


### Append new rule

```
iptables -A INPUT -p tcp --dport 8003 -j ACCEPT
```

#### Insert rule

The -I flag takes a chain and the rule position where you want to insert the new rule.

```
iptables -I INPUT -p tcp --dport 8003 -j ACCEPT
```

#### Remove the rule
```
iptables -D INPUT -p tcp --dport 8003 -j ACCEPT
```


#### Show current rules

```
iptables -S
```
