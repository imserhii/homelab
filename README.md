# home.lab

![Screenshot 2023-11-25 at 18 58 21](https://github.com/imserhii/homelab/assets/4532683/73ebe7bb-ef62-42a7-b3f0-c093aea7cc55)

### Requirements:
- Ansible
- Debian 12 (without setting root password)
- Melted brain

### How to run:
1. Add **secrets.yml** with **USER** and **PASSWORD** (and **PRINTER_IP** for Klipper)
2. Modify the hostname and IP in **inventory.cfg**
3. Add the machine as DNS to your router
4. `mkcert -cert-file cert.pem -key-file key.pem "*.home.lab" home.lab`
5. `ansible-playbook run.yml` → [home.lab](http://home.lab)
