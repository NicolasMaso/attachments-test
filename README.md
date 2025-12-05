# Attachments Test Repository

Este repositório contém arquivos de mídia públicos (imagens, áudios e PDFs) para uso em testes de integração.

## 📁 Estrutura do Repositório

```
attachments-test/
├── images/     # Imagens de teste (PNG, JPG)
├── audio/      # Arquivos de áudio (WAV, MP3)
└── pdfs/       # Documentos PDF
```

## 🖼️ Imagens Disponíveis

### PNG Images

| Arquivo | Dimensões | Cor | URL Raw |
|---------|-----------|-----|---------|
| `sample-image-1x1.png` | 1x1 | Cinza | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-image-1x1.png` |
| `sample-red-100x100.png` | 100x100 | Vermelho | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-red-100x100.png` |
| `sample-green-100x100.png` | 100x100 | Verde | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-green-100x100.png` |
| `sample-blue-100x100.png` | 100x100 | Azul | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-blue-100x100.png` |
| `sample-yellow-200x150.png` | 200x150 | Amarelo | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-yellow-200x150.png` |

### JPEG Images

| Arquivo | Dimensões | Cor | URL Raw |
|---------|-----------|-----|---------|
| `sample-image-1x1.jpg` | 1x1 | Cinza | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-image-1x1.jpg` |
| `sample-red-10x10.jpg` | 10x10 | Vermelho | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-red-10x10.jpg` |
| `sample-green-10x10.jpg` | 10x10 | Verde | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-green-10x10.jpg` |

## 🔊 Áudios Disponíveis

### WAV Files

| Arquivo | Duração | Frequência | URL Raw |
|---------|---------|------------|---------|
| `sample-tone-440hz-1sec.wav` | 1 segundo | 440 Hz (A4) | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/sample-tone-440hz-1sec.wav` |
| `sample-tone-440hz-half-sec.wav` | 0.5 segundos | 440 Hz (A4) | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/sample-tone-440hz-half-sec.wav` |
| `sample-tone-880hz-1sec.wav` | 1 segundo | 880 Hz (A5) | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/sample-tone-880hz-1sec.wav` |

### MP3 Files

| Arquivo | Descrição | URL Raw |
|---------|-----------|---------|
| `sample-silent.mp3` | Áudio silencioso | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/sample-silent.mp3` |

## 📄 PDFs Disponíveis

| Arquivo | Descrição | URL Raw |
|---------|-----------|---------|
| `sample-document.pdf` | Documento de teste simples | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/sample-document.pdf` |
| `sample-invoice.pdf` | Exemplo de fatura | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/sample-invoice.pdf` |
| `sample-report.pdf` | Exemplo de relatório | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/sample-report.pdf` |

## 🚀 Como Usar

### Acessar arquivos via URL Raw

Para usar estes arquivos em seus testes de integração, utilize as URLs Raw fornecidas nas tabelas acima. Por exemplo:

```javascript
// Exemplo em JavaScript
const imageUrl = 'https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-red-100x100.png';

fetch(imageUrl)
  .then(response => response.blob())
  .then(blob => {
    // Use o blob em seus testes
  });
```

```python
# Exemplo em Python
import requests

image_url = 'https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-red-100x100.png'
response = requests.get(image_url)

if response.status_code == 200:
    with open('test_image.png', 'wb') as f:
        f.write(response.content)
```

### Baixar arquivos localmente

```bash
# Baixar uma imagem
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/sample-red-100x100.png

# Baixar um áudio
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/sample-tone-440hz-1sec.wav

# Baixar um PDF
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/sample-document.pdf
```

## 📝 Notas

- Todos os arquivos são públicos e podem ser acessados sem autenticação
- As URLs Raw do GitHub são estáveis e podem ser usadas em ambientes de produção
- Os arquivos são simples e pequenos, ideais para testes automatizados
- Para usar em produção após merge, substitua `main` pelo nome da branch principal do repositório

## 🤝 Contribuindo

Para adicionar novos arquivos de teste:

1. Adicione o arquivo na pasta apropriada (`images/`, `audio/` ou `pdfs/`)
2. Atualize este README.md com as informações do novo arquivo
3. Commit e push suas alterações

## 📄 Licença

Domínio público - Use livremente para testes e desenvolvimento.