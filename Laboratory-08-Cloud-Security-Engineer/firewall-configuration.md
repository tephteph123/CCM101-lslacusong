# Firewall Configuration

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This rule allows SSH connections so administrators can manage the server remotely.

## 2. Set the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections unless a rule allows them. The second command allows outgoing connections from the server.

## 3. Enable UFW

```bash
sudo ufw enable
```

## 4. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This rule allows TCP traffic on port 8080 for the web application.

## 5. Verify Firewall Rules

```bash
sudo ufw status verbose
sudo ufw status numbered
```

These commands display the firewall status, default policies, and configured rules.

## 6. Why SSH Must Be Allowed First

If you run `sudo ufw enable` before `sudo ufw allow ssh`, the firewall may block your remote SSH connection and lock you out of the server.
