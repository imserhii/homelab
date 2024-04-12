# home.lab

<img width="1091" alt="Screenshot 2024-01-11 at 16 39 05" src="https://github.com/imserhii/homelab/assets/4532683/8ee1f817-8a80-45fd-932b-8d3fcdb7c17c">

### Requirements:
- Ansible
- Debian 12 (without setting root password)
- Melted brain

### How to run:
1. Add **secrets.yml** with:
    - *USERNAME*
    - *PASSWORD*
    - *HOST_IP*
    - *MAINSAIL_IP*
    - *GITEA_RUNNER_TOKEN*
    - *INFLUXDB_TOKEN*
    - *NTFY_URL*
2. Add the machine as DNS to your router
3. `mkcert -cert-file cert.pem -key-file key.pem "*.home.lab" home.lab`
4. `ansible-playbook run.yml` → [home.lab](https://home.lab)
