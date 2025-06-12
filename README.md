## 50% supply of $DGRAM for Node Operators.
[![IMG-20250612-132223-312.jpg](https://i.postimg.cc/hv4zRxmx/IMG-20250612-132223-312.jpg)](https://postimg.cc/8J3Ph7tP)

## 🚀 System Requirements

To ensure stable performance, we recommend the following VPS specifications:

| Component        | Recommended Specs        |
|------------------|--------------------------|
| CPU              | 2 vCPU (2+ GHz)          |
| RAM              | 8 GB RAM                 |
| Storage          | 20–25 GB SSD             |
| Operating System | Ubuntu 20.04 / 22.04 LTS |
| Bandwidth        | 1 TB/month or unlimited  |
| Uptime           | Must run 24/7            |

You can use VPS providers such as:
- 🌍 Contabo (affordable with high RAM)
- 🌐 Hetzner Cloud
- ☁️ DigitalOcean, Vultr, or Linode
- 🇮🇩 IDCloudHost or BiznetGio (Indonesia)


### 1️⃣ Download Datagram CLI

````
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux
````

### 2️⃣ Move the Binary

```bash
sudo mv datagram-cli-x86_64-linux /usr/local/bin/datagram-cli
```

### 3️⃣ Make It Executable

```bash
sudo chmod +x /usr/local/bin/datagram-cli
```

### 4️⃣ (Optional) Start a `screen` Session

```bash
screen -S datagram
```

This will allow the node to keep running even if your terminal is closed.

### 5️⃣ Run the Datagram Node

```bash
datagram-cli run -- -key YOUR_API_KEY
```

> 🔐 Replace `YOUR_API_KEY` with the key you can find in your **Wallet > Licenses > Key**.

---

## 📌 Command Summary

| Step | Command            | Description                                  |
| ---- | ------------------ | -------------------------------------------- |
| 1    | `wget`             | Downloads the CLI binary from GitHub         |
| 2    | `mv`               | Moves the binary to system's executable path |
| 3    | `chmod`            | Grants execute permissions to the binary     |
| 4    | `screen`           | Keeps your node running in the background    |
| 5    | `datagram-cli run` | Starts the Datagram node using your API key  |

---

## 🛠️ Tips

* Use `screen -r datagram` to reattach to the session if you disconnect.
* Use `CTRL+A + D` to detach safely without stopping the node.
* You can automate startup using `systemd` – ask if you'd like a service template.

