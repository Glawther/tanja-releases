# Tanja: versões e instaladores

Converta arquivos no **Windows** e no **Linux** sem abrir site nenhum: **arraste o arquivo, toque em Shift** (ou **Super+Z** no Wayland) e escolha o formato numa roda de vidro. Tudo é processado localmente no seu computador.

Baixe o instalador mais recente na aba [**Releases**](https://github.com/Glawther/tanja-releases/releases/latest). O app instalado verifica novas versões sozinho.

## Instalar no Windows

Baixe e execute **`Tanja-Setup-x.y.z.exe`** na aba [**Releases**](https://github.com/Glawther/tanja-releases/releases/latest).

## Instalar no Linux

### 1 comando (qualquer distribuição — detecta `.deb`, `.rpm`, `.pacman`, `.snap` ou `AppImage`)

```bash
curl -fsSL https://github.com/Glawther/tanja-releases/releases/latest/download/install-linux.sh | sh
```

### Ou escolha o pacote da sua distribuição na aba Releases:

```bash
# Debian, Ubuntu, Zorin OS, Linux Mint, Pop!_OS (.deb)
sudo apt install ./tanja_*_amd64.deb

# Fedora, RHEL, CentOS, Rocky, AlmaLinux (.rpm)
sudo dnf install ./tanja-*.x86_64.rpm

# openSUSE (.rpm)
sudo zypper install --allow-unsigned-rpm ./tanja-*.x86_64.rpm

# Arch Linux, Manjaro, EndeavourOS (.pacman)
sudo pacman -U ./tanja-*-x64.pacman

# Snap (Ubuntu, Zorin OS, Manjaro, Debian, Fedora...)
sudo snap install --dangerous ./tanja_*_amd64.snap

# AppImage universal (qualquer distribuição, atualiza sozinho)
chmod +x Tanja-*.AppImage && ./Tanja-*.AppImage
```

### Dica para sessões Wayland (Zorin OS, Ubuntu, GNOME, KDE...)

No Wayland, o sistema bloqueia a leitura global do Shift entre janelas. Por isso:
- No **GNOME / Zorin OS / Ubuntu**, o Tanja configura automaticamente o atalho **Super + Z** para abrir a roda (comece a arrastar o arquivo e aperte **Super + Z**, ou configure pelo ícone da bandeja).
- Em outros ambientes, associe um atalho do sistema ao comando `tanja --wheel`.
- Você também pode abrir a roda e **clicar diretamente numa fatia** para escolher o arquivo pelo seletor do sistema.