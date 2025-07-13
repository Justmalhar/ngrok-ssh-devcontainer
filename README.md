# 🚀 ngrok-ssh-devcontainer

A minimal development container with SSH access over Ngrok. Useful for remote access, live pair programming, or secure remote dev envs.

---

## 🛠 Features

- Ubuntu 20.04 base
- SSH server running
- Password login (can be upgraded to SSH key)
- Compatible with host Ngrok tunnel

---

## 🧪 Quickstart

### 1. Clone and build

```bash
git clone https://github.com/yourname/ssh-devcontainer.git
cd ssh-devcontainer
docker-compose up --build -d
```

### 2. Start Ngrok tunnel

Install Ngrok from [Ngrok](https://ngrok.com)

```bash
ngrok tcp 2222
```

Copy the public forwarding URL, e.g.

```
tcp://0.tcp.ngrok.io:12345
```

### 3. SSH into the container

```bash
ssh root@0.tcp.ngrok.io -p 12345
```

Password: `root`

---

## 🔐 To Do

- [ ] Add SSH key support
- [ ] Add VS Code Remote SSH compatibility
- [ ] Optional Docker volumes for code sharing

---

## 🧠 Notes

- Default user: `root`
- Default password: `root`
- Runs on port `2222` locally

Made by [@justmalhar](www.x.com/justmalhar)
