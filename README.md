# <p align="center">PyPhisher</p>

<p align="center">
  <img src="https://img.shields.io/badge/Versão-2.1.9-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Linguagem-Python-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Finalidade-Educacional-orange?style=for-the-badge">
</p>

<p align="center">
  <a href="https://gitlab.com/KasRoudra">
    <img src="https://img.shields.io/badge/Autor-KasRoudra-purple?style=flat-square">
  </a>
  <img src="https://img.shields.io/badge/Código_Aberto-Sim-cyan?style=flat-square">
  <img src="https://img.shields.io/badge/Origem-Bangladesh-green?style=flat-square">
</p>

---

## 📚 1. Descrição

O **PyPhisher** é uma ferramenta de código aberto desenvolvida em Python para demonstrar o funcionamento de técnicas de phishing e engenharia social.

O projeto apresenta recursos relacionados a páginas de autenticação, servidores web, tunelamento de conexões e análise de mecanismos de captura de informações.

**Este repositório destina-se exclusivamente a fins estudantis, pesquisas acadêmicas, auditorias autorizadas e atividades educacionais de Segurança da Informação.**

Seu principal objetivo educacional é contribuir para a compreensão das ameaças digitais e o desenvolvimento de estratégias de prevenção e proteção.

> [!IMPORTANT]
> **USO EXCLUSIVAMENTE EDUCACIONAL**
>
> O estudo do projeto deve ocorrer em ambientes controlados e autorizados.
>
> A utilização de páginas fraudulentas para obter credenciais ou informações pessoais sem autorização pode constituir atividade ilícita.

### Continuidade do projeto

O desenvolvedor original informou que o PyPhisher passou a integrar o projeto [MaxPhisher](https://gitlab.com/KasRoudra/MaxPhisher), no qual seriam disponibilizadas novas funcionalidades e correções.

---

## 🎯 2. Objetivos educacionais

- Compreender o funcionamento de ataques de phishing.
- Identificar páginas falsas e tentativas de engenharia social.
- Analisar códigos Python, PHP, HTML e JavaScript.
- Estudar mecanismos de autenticação e proteção de credenciais.
- Compreender o funcionamento de servidores web e túneis de rede.
- Identificar riscos associados à exposição de informações pessoais.
- Desenvolver estratégias de defesa contra fraudes digitais.
- Aplicar conhecimentos de Redes de Computadores e Cibersegurança.
- Incentivar o uso ético e responsável de ferramentas de segurança.

---

## ⚙️ 3. Características do projeto

Entre os recursos descritos pelo desenvolvedor original estão:

- Compatibilidade com diferentes distribuições Linux.
- Interface de execução pelo terminal.
- Biblioteca de modelos de páginas web.
- Suporte a parâmetros de execução.
- Recursos de tunelamento.
- Simulações de páginas de autenticação.
- Suporte a modelos de autenticação OTP.
- Configurações de redirecionamento.
- Recursos de manipulação e pré-visualização de URLs.
- Registro de informações de acesso.
- Recursos de análise de erros.
- Disponibilização por Git, Python e Docker.

> [!WARNING]
> Essas funcionalidades devem ser estudadas exclusivamente em ambientes controlados e autorizados. Não utilize páginas simuladas para coletar credenciais reais ou enganar terceiros.

---

## 💻 4. Requisitos técnicos

### Linguagem principal

- Python 3

### Bibliotecas Python

- `requests`
- `rich`
- `beautifulsoup4`

### Outros componentes

- Git
- PHP
- SSH
- Ambiente Linux ou máquina virtual
- Aproximadamente 900 MB de armazenamento, conforme a documentação original

### Sistemas operacionais

| Sistema | Compatibilidade informada |
|---|---|
| Linux | Excelente |
| Android / Termux | Excelente |
| macOS | Experimental |
| iOS | Experimental |
| Windows | Por máquina virtual ou Docker |
| BSD | Não testado |

As informações de compatibilidade foram baseadas na documentação original e podem variar conforme a versão do projeto.

---

## 🛠️ 5. Instalação e preparação do ambiente

O PyPhisher foi desenvolvido em Python e possui suporte documentado para diferentes distribuições GNU/Linux e ambientes Termux.

### 5.1. Instalação das dependências

Instale os componentes necessários conforme o sistema operacional utilizado.

#### 🐧 Debian, Ubuntu, Kali Linux e Parrot OS

```bash
sudo apt update
sudo apt install git python3 python3-pip php openssh-client -y
```

#### 🐧 Arch Linux e Manjaro

```bash
sudo pacman -S git python python-pip php openssh --noconfirm
```

#### 🐧 Fedora e distribuições baseadas em Red Hat

```bash
sudo dnf install git python3 python3-pip php openssh-clients -y
```

#### 📱 Android — Termux

```bash
pkg update && pkg upgrade -y
pkg install git python php openssh -y
```

> [!NOTE]
> Os nomes dos pacotes podem variar conforme a distribuição Linux e a versão do sistema operacional.

### 5.2. Clonagem do repositório

**Repositório original:**

```bash
git clone https://gitlab.com/KasRoudra/PyPhisher.git
```

**Repositório de referência da adaptação:**

```bash
git clone https://github.com/profjvidal/PyPhisher.git
```

Escolha apenas um dos repositórios.

### 5.3. Acessar o diretório

```bash
cd PyPhisher
```

### 5.4. Examinar os arquivos

```bash
ls -la
```

###
