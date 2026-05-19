# Kali Linux for Radxa Dragon Q6A (Ready to Use)

[English]
This is a customized Kali Linux image optimized for the Radxa Dragon Q6A single-board computer. The image has been surgically shrunk to provide a fast download and minimize storage requirements before installation.

---

### EN
## 🚀 How to Install

1. Download all split files (`.00`, `.01`) and the `SHA256SUMS` file from the **Releases** section.
2. Verify the file integrity by running:
   ```bash
   sha256sum -c SHA256SUMS
3. Join the split files back into a single compressed image:
   ```bash
   cat kali-radxa-dragon-q6a.img.xz.* > kali-radxa-dragon-q6a.img.xz
4. Flash the image to your SSD using your preferred tool (e.g., `dd`, BalenaEtcher, or Raspberry Pi Imager).
5. Connect the SSD to your Radxa Dragon Q6A and power on the device.

## 💾 Expanding Disk Space / Expandindo o Espaço do Disco
To keep the download lightweight (only ~3GB), the default filesystem is constrained. On the first boot, the partition layout will automatically scale to match your SSD size. However, to make Kali recognize the full capacity of your drive, open the terminal and execute the following command:
```bash
sudo resize2fs /dev/nvme0n1p3
``` 
After execution, the full capacity of your SSD will be completely available for use.

## ⚖️ License 
This project is licensed under the MIT License - see the LICENSE file for details.

---

# Imagem do Kali Linux para Radxa Dragon Q6A (Pronta para Uso)

[Português]
Esta é uma imagem customizada do Kali Linux otimizada para o computador de placa única Radxa Dragon Q6A. A imagem foi reduzida de forma cirúrgica para fornecer um download rápido e minimizar os requisitos de armazenamento antes da instalação.

---

### PT-BR
## 🚀 Como Instalar

1. Baixe todas as partes divididas (`.00`, `.01`) e o arquivo `SHA256SUMS` na seção de Releases.
2. Verifique a integridade dos arquivos executando:
   ```bash
   sha256sum -c SHA256SUMS
3. Junte as partes de volta em uma única imagem compactada:
   ```bash
   cat kali-radxa-dragon-q6a.img.xz.* > kali-radxa-dragon-q6a.img.xz
4. Grave a imagem no seu SSD utilizando uma ferramenta de sua preferência (ex: `dd`, BalenaEtcher ou Raspberry Pi Imager).
5. Conecte o SSD no seu Radxa Dragon Q6A e ligue a placa.

## 💾 Expandindo o Espaço do Disco

Para manter a imagem leve (apenas ~3GB de download), o sistema de arquivos padrão está limitado. No primeiro boot, o layout da partição será esticado automaticamente para corresponder ao tamanho do seu SSD. No entanto, para que o Kali reconheça toda a capacidade do seu disco, abra o terminal e execute o seguinte comando:
```bash
sudo resize2fs /dev/nvme0n1p3
```
Após a execução, o espaço total do seu SSD estará completamente liberado para uso.

## ⚖️ Licença
Este projeto está licenciado sob a Licença MIT - consulte o arquivo LICENSE para mais detalhes.
