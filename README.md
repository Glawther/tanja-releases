# Tanja: versões e instaladores

Converta arquivos no **Windows** e no **Linux** sem abrir site nenhum: **arraste o arquivo, toque em Shift** (ou no botão/atalho de sua escolha) e escolha o formato numa roda de vidro. Tudo é processado localmente no seu computador.

Baixe o instalador mais recente na aba [**Releases**](https://github.com/Glawther/tanja-releases/releases/latest). O app instalado verifica novas versões sozinho.

## Escolher qual ou quais botões abrem a roda

No ícone da bandeja do sistema → **Botões para abrir a roda**, você pode:
- **Marcar um ou vários botões ao mesmo tempo:** `Shift` (padrão), `Ctrl`, `Alt`, `Tecla Windows / Super`, `Barra de Espaço`, `Tab`, `Caps Lock`, `Botão do meio do mouse (Scroll)` ou `Botões laterais do mouse (4 e 5)`.
- **Gravar outra tecla ou botão:** clique em *"Gravar outra tecla ou botão…"* e aperte qualquer tecla do teclado ou botão do mouse para usá-lo.
- **Atalho do sistema (Wayland / GNOME):** escolha entre `Super + Z`, `Alt + Z`, `Ctrl + Espaço`, `Super + Espaço`, `F8` e `F9`.

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

### Dica para sessões Wayland (Fedora, Zorin OS, Ubuntu, GNOME, KDE...)

- Tanto o **Shift** (ou a tecla escolhida no menu) quanto o atalho **Super + Z** abrem a roda no centro da tela.
- Você também pode abrir a roda e **clicar diretamente numa fatia** para escolher o arquivo pelo seletor do sistema.