# 📚 Librería Misteriosa — VM Pentest Lab (Docker)

**Descripción**\
“Librería Misteriosa” es un laboratorio de pentesting web basado en Docker, inspirado en una antigua librería de manuscritos arcanos. Recorre desde la fase de reconocimiento hasta escalada de privilegios:

---

## 📦 Releases

Descarga la imagen Docker empaquetada desde la sección **Releases** de GitHub:

[Releases – Librería Misteriosa](https://github.com/dani-18/Libreria-Misteriosa-VM-Lab/releases)

---

## ⚙️ Requisitos

- Docker >= 19.03
- (Opcional) `bash` en tu sistema host para poder desplegar `auto_deploy.sh`

---

## 🚀 Despliegue automático

1. **Descarga** el ZIP desde la release del repositorio:
   ```bash
   git clone https://github.com/TU_USUARIO/libreria-misteriosa.git
   cd libreria-misteriosa
   ```
2. **Descomprime** el ZIP descargado:
   ```bash
   unzip libreria_misteriosa.zip
   ```
3. **Da permisos** de ejecución al instalador:
   ```bash
   chmod +x auto_deploy.sh
   ```
4. **Ejecuta** el instalador:
   ```bash
   ./auto_deploy.sh
   ```

---

## 🧨 Vulnerabilidades

- Login vulnerable a fuerza bruta
- RCE mediante subida de imágenes (polyglot JPEG+PHP)
- Extracción de hash Bcrypt desde metadatos EXIF
- Escalada www-data → librarian rompiendo hash con rockyou
- Escalada librarian → root vía cron-job Python editable

> Este repositorio es únicamente para fines educativos. No desplegar en entornos de producción.

