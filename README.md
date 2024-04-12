# home.lab

<img width="1223" alt="Screenshot 2024-04-12 at 15 10 58" src="https://github.com/imserhii/homelab/assets/4532683/c0d51ace-6a50-4ac6-a2e8-730a1c7f3bc2">

### Requirements:
- Ansible
- Debian 12 (without setting root password)
- Melted brain

### How to run:
1. Add **secrets.yml** with:
    - *USERNAME*
    - *PASSWORD*
    - *HOST_IP*
    - *EXTERNAL_HOSTNAME*
    - *MAINSAIL_IP*
    - *GITEA_RUNNER_TOKEN*
    - *INFLUXDB_TOKEN*
    - *RCLONE_CLIENT_ID*
    - *RCLONE_CLIENT_SECRET*
    - *RCLONE_TOKEN*
2. Add the machine as DNS to your router
3. `mkcert -cert-file cert.pem -key-file key.pem "*.home.lab" home.lab`
4. `ansible-playbook run.yml` → [home.lab](https://home.lab)
