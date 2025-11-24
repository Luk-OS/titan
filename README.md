
# Repositorio APT de Titan

Este repositorio contiene paquetes `.deb`, hosteado en GitHub Pages.

---

🛠️ Instalación

### 1️⃣ Añadir la clave GPG
```bash
sudo mkdir -p /usr/share/keyrings
wget -qO - https://luk-os.github.io/titan/public.key | sudo gpg --dearmor -o /usr/share/keyrings/titan.gpg
```

### 2️⃣ Añadir el repositorio
```bash
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/titan.gpg trusted=yes] https://luk-os.github.io/titan/ stable main"     | sudo tee /etc/apt/sources.list.d/titan.list

sudo apt update --allow-insecure-repositories
```

### 3️⃣ Instalar paquetes
```bash
sudo apt install nombre-del-paquete
```
