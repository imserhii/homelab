# home.lab

![Screenshot 2023-11-25 at 18 58 21](https://github.com/imserhii/homelab/assets/4532683/73ebe7bb-ef62-42a7-b3f0-c093aea7cc55)

### Requirements:
- Ansible
- Debian 12 (without setted root password)
- Melted brain

### How to run:
1. Add **creds.yml** with your `USER` and `PASSWORD`
2. Modify the hostname and IP in **inventory.cfg**
3. `ansible-playbook run.yml`
4. Add the machine as a DNS server to your router
5. → [home.lab](http://home.lab)

> P.S. Yeah, I don't care about HTTPS and "0". Only VPN, and only hardcore!
