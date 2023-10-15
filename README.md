# Cloud City Crafted GitHub Actions Ubuntu Runner Images

This image can be used to emulate a GitHub Action runner for `ubuntu-latest` or a small Ubuntu container. It is also compatible with [act](https://github.com/nektos/act) as alternative runner images.

## 🖥️ System Information

- Base Image: [ubuntu:latest](https://hub.docker.com/layers/library/ubuntu/latest/images/sha256-b492494d8e0113c4ad3fe4528a4b5ff89faa5331f7d52c5c138196f69ce176a6?context=explore)
- OS: Ubuntu 22.04.3 LTS
- Codename: Jammy Jellyfish
- Kernel: Linux 6.3.13-linuxkit x86_64

## 📋 Package Repositories

- [Node.js DEB repository](https://deb.nodesource.com)

## 📦 Packages

- ca-certificates
- curl
- gh
- git
- gnupg
- lsb-release
- nodejs
- pipx
- python3
- python3-pip
- python3-venv
- zstd

## ⚙️ Environment Variables

| Name           | Value              |
| -------------- | ------------------ |
| `NODE_MAJOR`   | `16`               |
| `PIPX_BIN_DIR` | `"/usr/local/bin"` |

## 🗂️ Configuration Files

### 🔑 GPG

Configures GPG to allow passphrases to be preset to avoid interactive prompting

Location: `"$HOME/.gnupg/gpg-agent.conf"`

```shell
default-cache-ttl 21600
allow-preset-passphrase
```

### 🔐 SSH

Configures SSH to trust [GitHub SSH Key Fingerprints](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/githubs-ssh-key-fingerprints)

Location: `"$HOME/.ssh/known_hosts"`

```shell
github.com ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIOMqqnkVzrm0SdG6UOoqKLsabgH5C9okWi0dh2l9GKJl
github.com ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBEmKSENjQEezOmxkZMy7opKgwFB9nkt5YRrYMjNuG5N87uRgg6CLrbo5wAdT/y6v0mKV0U2w0WZ2YB/++Tpockg=
github.com ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCj7ndNxQowgcQnjshcLrqPEiiphnt+VTTvDP6mHBL9j1aNUkY4Ue1gvwnGLVlOhGeYrnZaMgRK6+PKCUXaDbC7qtbW8gIkhL7aGCsOr/C56SJMy/BCZfxd1nWzAOxSDPgVsmerOBYfNqltV9/hWCqBywINIR+5dIg6JTJ72pcEpEjcYgXkE2YEFXV1JHnsKgbLWNlhScqb2UmyRkQyytRLtL+38TGxkxCflmO+5Z8CSSNY7GidjMIZ7Q4zMjA2n1nGrlTDkzwDCsw+wqFPGQA179cnfGWOWRVruj16z6XyvxvjJwbz0wQZ75XK5tKSb7FNyeIEs4TT4jk+S4dhPeAUC5y+bDYirYgM4GC7uEnztnZyaVWQ7B381AK4Qdrwt51ZqExKbQpTUNn+EjqoTwvqNj4kqx5QUCI0ThS/YkOxJCXmPUWZbhjpCg56i+2aB6CmK2JGhn57K5mj0MNdBXA4/WnwH6XoPWJzK5Nyu2zB3nAZp+S5hpQs+p1vN1/wsjk=
```

## 🧑🏽‍💻 Contributing

See [Cloud City Crafted Container Images Contributing Guide](https://github.com/cloud-city-crafted-images/.github-private/tree/main/profile).

## 🪪 License

This repository is [MIT licensed](./LICENSE).
