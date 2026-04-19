<div align="center">

# ▶ YouDown
### YouTube Downloader para Windows

![Java](https://img.shields.io/badge/Java-11%2B-orange?style=flat-square&logo=java)
![License](https://img.shields.io/badge/Licença-MIT-blue?style=flat-square)
![Platform](https://img.shields.io/badge/Plataforma-Windows-lightgrey?style=flat-square&logo=windows)
![yt-dlp](https://img.shields.io/badge/powered%20by-yt--dlp-red?style=flat-square)

Interface gráfica moderna e simples para baixar vídeos e áudios do YouTube usando **yt-dlp** e **FFmpeg**.

</div>

---

## 📸 Funcionalidades

- 🎬 Download de vídeos em **MP4** (melhor qualidade disponível)
- 🎵 Extração de áudio em **MP3**, **M4A** ou **WAV**
- 📋 **Fila de downloads** com progresso em tempo real (velocidade, ETA, tamanho)
- 📁 Escolha a **pasta de destino** para cada download
- 🍪 Suporte a **cookies** do YouTube (vídeos com restrição de idade)
- 🔄 Downloads **simultâneos** configuráveis (1 a 5)
- 📥 **Instalação automática do FFmpeg** diretamente pelo app
- 🌍 Adição automática ao **PATH do Windows**
- 🎨 Interface escura moderna com **FlatLaf**
- 🔒 Executa como **Administrador** automaticamente

---

## 🚀 Como usar

### Pré-requisitos

| Requisito | Download | Obrigatório |
|-----------|----------|-------------|
| **Java 11+** | [Adoptium](https://adoptium.net/) | ✅ Sim |
| **yt-dlp** | [Releases](https://github.com/yt-dlp/yt-dlp/releases) | ✅ Sim |
| **FFmpeg** | Instalado pelo próprio YouDown | ✅ Sim |

### Instalação

1. Baixe o `YouDown.exe` na seção [Releases](../../releases)
2. Coloque o `yt-dlp.exe` na **mesma pasta** do `YouDown.exe`
3. Execute o `YouDown.exe` como **Administrador**
4. Na primeira abertura, o app detecta e instala o **FFmpeg automaticamente**

### Estrutura de pastas recomendada

```
📁 YouDown/
├── YouDown.exe          ← executável principal
├── yt-dlp.exe           ← baixe em github.com/yt-dlp/yt-dlp/releases
├── ffmpeg.exe           ← instalado automaticamente pelo YouDown
└── youtube_cookies.txt  ← opcional, para vídeos restritos
```

---

## 🍪 Usando Cookies (opcional)

Para baixar vídeos com restrição de idade ou conteúdo privado:

1. Instale a extensão **[Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc)** no Chrome ou Firefox
2. Acesse o YouTube estando logado
3. Clique na extensão e exporte os cookies
4. No YouDown, vá em **Configurações → Cookies** e aponte para o arquivo exportado

---

## ⚙️ Configurações disponíveis

| Configuração | Descrição |
|---|---|
| Caminho do yt-dlp | Caminho personalizado ou usa o PATH |
| FFmpeg | Instalação e gerenciamento automático |
| Cookies | Arquivo de cookies para conteúdo restrito |
| Pasta padrão | Destino padrão dos downloads |
| Downloads simultâneos | De 1 a 5 downloads ao mesmo tempo |
| Formato padrão | MP4, MP3, M4A, WAV ou Melhor Qualidade |

---

## 🛠️ Compilando o projeto

### Requisitos de desenvolvimento

- Java JDK 11+
- Maven 3.6+
- IntelliJ IDEA / Eclipse / NetBeans

### Build

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/YouDown.git
cd YouDown

# Compilar e gerar JAR
mvn clean package

# O JAR estará em:
# target/YouDown.jar
```

### Gerando o EXE (Launch4j)

1. Instale o [Launch4j](https://launch4j.sourceforge.net/)
2. Abra o arquivo `launch4j-config.xml` incluído no projeto
3. Clique em **Build Wrapper**
4. O `YouDown.exe` será gerado na pasta raiz

---

## 📦 Tecnologias utilizadas

| Tecnologia | Versão | Descrição |
|---|---|---|
| [Java](https://adoptium.net/) | 11+ | Linguagem principal |
| [FlatLaf](https://www.formdev.com/flatlaf/) | 3.4 | Tema moderno para Swing |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | latest | Motor de download |
| [FFmpeg](https://ffmpeg.org/) | latest | Conversão de mídia |
| [Launch4j](https://launch4j.sourceforge.net/) | 3.50 | Gerador de EXE |

---

## ⚖️ Termos de Uso e Responsabilidade

> **Aviso importante:** Este software destina-se **exclusivamente** ao download de conteúdos de domínio público ou com autorização expressa do detentor dos direitos autorais.

- O YouDown **não hospeda** nenhum conteúdo
- O YouDown **não coleta** dados dos usuários
- O usuário é **inteiramente responsável** pelo uso do software
- Baixar conteúdo protegido por direitos autorais sem permissão pode violar leis locais e os Termos de Serviço das plataformas

Leia os [Termos de Uso completos](TERMS.md) antes de usar.

---

## ☕ Apoie o Projeto

O YouDown é **gratuito e sem anúncios**. Se ele te ajudou, considere fazer uma doação para manter o projeto vivo e atualizado!

<div align="center">

### 💛 PIX

**Chave PIX (Telefone):**
```
5573991707161
```
**Favorecido:** Guilherme Sampaio

---

### 🅿 PayPal

[![PayPal](https://img.shields.io/badge/Doar%20via%20PayPal-0070BA?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/donate/?business=guilhermesampaio.adm%40gmail.com&currency_code=BRL)

`guilhermesampaio.adm@gmail.com`

---

Ou pelo WhatsApp:

[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B55%2073%2099170--7161-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/5573991707161)

</div>


---

## 📄 Licença

Este projeto está licenciado sob a **Licença MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

```
MIT License — Você pode usar, copiar, modificar e distribuir este software
livremente, desde que mantenha os créditos ao desenvolvedor original.
```

---

## 👨‍💻 Desenvolvedor

<div align="center">

**Guilherme Sampaio**

[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B55%2073%2099170--7161-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/5573991707161)
[![Gmail](https://img.shields.io/badge/Gmail-guilhermesampaio.adm%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:guilhermesampaio.adm@gmail.com)

</div>

---

<div align="center">
Feito com ❤️ por <b>Guilherme Sampaio</b>
</div>