
# UFW Firewall Command Module

## Installing and Setting Up UFW
- **Install UFW**: 
  ```bash
  sudo apt install ufw
  ```
- **Enable UFW**:
  ```bash
  sudo ufw enable
  ```
- **Set Default Policies**:
  ```bash
  sudo ufw default deny incoming
  sudo ufw default allow outgoing
  ```

## Starting, Stopping, and Reloading UFW
- **Start UFW**:
  ```bash
  sudo ufw enable
  ```
- **Stop UFW**:
  ```bash
  sudo ufw disable
  ```
- **Reload UFW**:
  ```bash
  sudo ufw reload
  ```

## Allowing and Denying Traffic
- **Allow Traffic on a Specific Port**:
  ```bash
  sudo ufw allow [port]/[protocol]
  ```
- **Deny Traffic on a Specific Port**:
  ```bash
  sudo ufw deny [port]/[protocol]
  ```
- **Allow Traffic from a Specific IP Address**:
  ```bash
  sudo ufw allow from [IP_address]
  ```
- **Deny Traffic from a Specific IP Address**:
  ```bash
  sudo ufw deny from [IP_address]
  ```

## Checking UFW Status and Rules
- **Basic UFW Status**:
  ```bash
  sudo ufw status
  ```
- **Verbose UFW Status**:
  ```bash
  sudo ufw status verbose
  ```
- **UFW Status with Numbers**:
  ```bash
  sudo ufw status numbered
  ```

## Additional Commands for Network Status (Outside UFW Perspective)
- **List All Open Ports**:
  ```bash
  sudo ss -tuln
  ```
- **List Open TCP Ports**:
  ```bash
  sudo ss -tuln | grep 'tcp'
  ```
- **List Open UDP Ports**:
  ```bash
  sudo ss -tuln | grep 'udp'
  ```

### Implementation Notes
- Most UFW commands require superuser privileges.
- For allow/deny commands, `[protocol]` can be `tcp`, `udp`, or omitted for both.
- Replace `[port]` with the actual port number and `[IP_address]` with the actual IP address.
