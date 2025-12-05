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

| Arquivo                      | Descrição              | URL Raw                                                                                                 |
| ---------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------- |
| `comprovante-falso.png`      | Comprovante falso      | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/comprovante-falso.png`      |
| `comprovante-verdadeiro.png` | Comprovante verdadeiro | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/comprovante-verdadeiro.png` |

## 🔊 Áudios Disponíveis

| Arquivo            | Descrição          | URL Raw                                                                                      |
| ------------------ | ------------------ | -------------------------------------------------------------------------------------------- |
| `cobrando-pix.mp3` | Áudio cobrando pix | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/cobrando-pix.mp3` |

## 📄 PDFs Disponíveis

| Arquivo                      | Descrição              | URL Raw                                                                                               |
| ---------------------------- | ---------------------- | ----------------------------------------------------------------------------------------------------- |
| `comprovante-falso.pdf`      | Comprovante falso      | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/comprovante-falso.pdf`      |
| `comprovante-verdadeiro.pdf` | Comprovante verdadeiro | `https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/comprovante-verdadeiro.pdf` |

## 🚀 Como Usar

### Acessar arquivos via URL Raw

Para usar estes arquivos em seus testes de integração, utilize as URLs Raw fornecidas nas tabelas acima.

### Baixar arquivos localmente

```bash
# Baixar uma imagem
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/images/comprovante-verdadeiro.png

# Baixar um áudio
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/audio/cobrando-pix.mp3

# Baixar um PDF
curl -O https://raw.githubusercontent.com/NicolasMaso/attachments-test/main/pdfs/comprovante-verdadeiro.pdf
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
