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

### 5.5. Consultar as dependências

```bash
cat files/requirements.txt
```

### 5.6. Criar um ambiente virtual Python

Recomenda-se utilizar um ambiente virtual para evitar conflitos com as bibliotecas do sistema.

```bash
python3 -m venv .venv
```

Ative o ambiente:

```bash
source .venv/bin/activate
```

Em sistemas Debian e Ubuntu, pode ser necessário instalar previamente o pacote `python3-venv`.

### 5.7. Instalar os módulos Python

Após revisar as dependências:

```bash
python3 -m pip install -r files/requirements.txt
```

> [!TIP]
> A utilização de um ambiente virtual dispensa normalmente o parâmetro `--break-system-packages`, evitando modificações desnecessárias no ambiente Python gerenciado pelo sistema operacional.

### 5.8. Verificar a sintaxe do código-fonte

Antes de executar programas obtidos de repositórios externos, recomenda-se analisar seus arquivos.

O exemplo abaixo realiza uma verificação sintática do arquivo principal sem executá-lo:

```bash
python3 - <<'PY'
import ast
from pathlib import Path

arquivo = Path("pyphisher.py")

ast.parse(arquivo.read_text(encoding="utf-8"))

print("Análise sintática concluída com sucesso.")
PY
```

**Importante:** a verificação sintática não garante que o programa seja seguro. Ela apenas verifica se o arquivo pode ser interpretado sintaticamente como código Python.

### 5.9. Instalação por Pip

A documentação original também apresenta a distribuição do projeto por meio do gerenciador de pacotes Pip.

Para consultar as versões disponíveis:

```bash
python3 -m pip index versions pyphisher
```

Antes de instalar um pacote, verifique sua procedência, versão, dependências e licença.

### 5.10. Docker

O projeto original também menciona a imagem Docker:

`kasroudra/pyphisher`

Para verificar a disponibilidade do manifesto da imagem:

```bash
docker manifest inspect kasroudra/pyphisher
```

A utilização de contêineres deve observar as políticas de segurança do laboratório.

### 5.11. Execução em laboratório

O arquivo principal identificado na documentação original é:

`pyphisher.py`

O estudo deve priorizar a análise estática, o entendimento das dependências e a investigação dos mecanismos de autenticação e comunicação.

A inicialização de funcionalidades capazes de reproduzir páginas fraudulentas ou coletar credenciais deve permanecer restrita a atividades especificamente autorizadas e supervisionadas.

> [!CAUTION]
> Não utilize o projeto para disponibilizar páginas fraudulentas publicamente ou obter credenciais de terceiros.

---

## 🔐 6. Ambiente de laboratório

Para atividades acadêmicas, recomenda-se:

1. Utilizar máquinas virtuais isoladas.
2. Trabalhar com páginas demonstrativas próprias.
3. Utilizar exclusivamente usuários e senhas fictícios.
4. Evitar exposição dos serviços à Internet pública.
5. Não utilizar contas reais de terceiros.
6. Registrar as autorizações necessárias.
7. Analisar o tráfego de rede em ambiente controlado.
8. Remover os dados de teste após as atividades.

### Recomendações adicionais

- Priorizar redes internas e ambientes sem acesso externo.
- Manter registros das atividades acadêmicas.
- Monitorar os serviços utilizados.
- Evitar o armazenamento desnecessário de informações.
- Respeitar as normas institucionais de segurança.

---

## 🧪 7. Aplicações educacionais

### Redes de Computadores

Estudo de protocolos HTTP/HTTPS, endereçamento IP, portas, servidores web e tunelamento.

### Segurança da Informação

Estudo de autenticação, proteção de credenciais, engenharia social e prevenção de fraudes.

### Programação

Análise e interpretação de códigos Python, PHP, HTML e JavaScript.

### Cibersegurança

Análise estática de software, identificação de comportamentos suspeitos e investigação de páginas fraudulentas.

### Ética e legislação digital

Discussão sobre privacidade, responsabilidade profissional, autorização para testes e limites legais das atividades de segurança cibernética.

---

## ⚖️ 8. Legislação brasileira aplicável

A utilização de ferramentas de segurança cibernética deve respeitar a legislação brasileira.

### Lei nº 12.737/2012 — Lei Carolina Dieckmann

Introduziu dispositivos no Código Penal relacionados a delitos informáticos, incluindo o artigo 154-A.

**Fonte oficial:**

https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2012/lei/l12737.htm

### Lei nº 14.155/2021

Alterou dispositivos do Código Penal relacionados à invasão de dispositivo informático, furto e estelionato, incluindo situações envolvendo meios eletrônicos.

**Fonte oficial:**

https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2021/lei/l14155.htm

### Lei nº 12.965/2014 — Marco Civil da Internet

Estabelece princípios, garantias, direitos e deveres para o uso da Internet no Brasil.

**Fonte oficial:**

https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/lei/l12965.htm

### Lei nº 13.709/2018 — Lei Geral de Proteção de Dados Pessoais (LGPD)

Estabelece regras para o tratamento de dados pessoais, incluindo princípios de segurança, privacidade e proteção de informações.

**Fonte oficial:**

https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm

### Decreto-Lei nº 2.848/1940 — Código Penal Brasileiro

Destacam-se:

- **Artigo 154-A:** invasão de dispositivo informático.
- **Artigo 171:** estelionato, incluindo disposições relacionadas à fraude eletrônica.

**Fonte oficial:**

https://www.planalto.gov.br/ccivil_03/decreto-lei/del2848compilado.htm

> [!WARNING]
> **RESPONSABILIDADE LEGAL**
>
> A finalidade educacional não autoriza automaticamente o acesso a sistemas, a coleta de credenciais ou o tratamento de dados pessoais.
>
> Dependendo das circunstâncias, atividades realizadas sem autorização podem gerar responsabilização civil e criminal.

---

## 📋 9. Termo de responsabilidade e uso ético

A utilização deste projeto deve respeitar os seguintes princípios:

1. **Autorização:** realizar testes somente em sistemas próprios ou expressamente autorizados.
2. **Privacidade:** respeitar os direitos e a proteção de dados pessoais.
3. **Legalidade:** cumprir a legislação brasileira e as normas institucionais.
4. **Ética:** não utilizar a ferramenta para fraudes ou obtenção indevida de informações.
5. **Segurança:** manter as atividades restritas a ambientes controlados.
6. **Responsabilidade:** documentar os procedimentos e prevenir impactos sobre terceiros.

É proibida, no contexto educacional desta adaptação, a utilização para roubo de senhas, invasões, falsificação de identidade ou qualquer outra atividade ilícita.

---

## 👨‍💻 10. Créditos e reconhecimento

### Desenvolvedor original

**KasRoudra**

- **GitLab:** https://gitlab.com/KasRoudra
- **GitHub:** https://github.com/KasRoudra
- **PyPhisher:** https://gitlab.com/KasRoudra/PyPhisher
- **MaxPhisher:** https://gitlab.com/KasRoudra/MaxPhisher

### Repositório de referência

**profjvidal/PyPhisher**

https://github.com/profjvidal/PyPhisher

### Reconhecimento de autoria

Todos os direitos autorais e créditos de desenvolvimento pertencem aos respectivos autores.

Esta adaptação possui finalidade exclusivamente acadêmica e educacional, não reivindicando autoria sobre o código-fonte original.

As modificações e redistribuições devem respeitar a licença original e preservar os avisos de direitos autorais aplicáveis.

---

## ⚠️ 11. Aviso legal

**ESTE REPOSITÓRIO É DESTINADO EXCLUSIVAMENTE A FINS EDUCACIONAIS E DE PESQUISA EM SEGURANÇA DA INFORMAÇÃO.**

O material tem como finalidade contribuir para o estudo de ameaças digitais, identificação de vulnerabilidades e desenvolvimento de estratégias de defesa cibernética.

A disponibilização do código não representa autorização para invasões, fraudes eletrônicas, captura indevida de credenciais, violação de privacidade ou outras atividades ilícitas.

A responsabilidade pela utilização do software cabe a quem realiza os respectivos atos, conforme a legislação aplicável.

O mantenedor desta adaptação não reivindica a autoria do projeto original nem declara vínculo com seu desenvolvedor.

---

## 📚 12. Referências complementares

- [CERT.br — Centro de Estudos, Resposta e Tratamento de Incidentes de Segurança no Brasil](https://www.cert.br/)
- [Cartilha de Segurança para Internet](https://cartilha.cert.br/)
- [OWASP — Open Worldwide Application Security Project](https://owasp.org/)
- [NIC.br — Núcleo de Informação e Coordenação do Ponto BR](https://www.nic.br/)
- [Python — Documentação oficial](https://docs.python.org/3/)
- [Planalto — Legislação brasileira](https://www.planalto.gov.br/)

---

<p align="center">
  <strong>Segurança da Informação • Redes de Computadores • Cibersegurança • Educação Digital</strong>
</p>

<p align="center">
  <em>Conhecer as ameaças digitais é essencial para desenvolver estratégias de prevenção e proteção.</em>
</p>
