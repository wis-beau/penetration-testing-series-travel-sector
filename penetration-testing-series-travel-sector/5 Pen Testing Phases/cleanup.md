### 📄 `cleanup.md`

# Covering Tracks (Red Team Simulation)

- Cleared `.bash_history`:

cat /dev/null > ~/.bash_history

- Deleted uploaded reverse shell after session closed

- Modified access logs to remove attacker IP:
sed -i '/attacker-ip/d' /var/log/apache2/access.log


