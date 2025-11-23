
# Repositorio APT de Titan
### 1️⃣ Añadir GPG
```bash
wget -qO - https://luk-os.github.io/titan/public.key | sudo gpg --dearmor -o /usr/share/keyrings/titan.gpg
```
### 2️⃣ Añadir Repo
```bash
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/titan.gpg trusted=yes] https://luk-os.github.io/titan/ stable main" | sudo tee /etc/apt/sources.list.d/titan.list
sudo apt update --allow-insecure-repositories
```
