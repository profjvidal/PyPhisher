<h1 align="center">PyPhisher</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Versão-2.1.9-green?style=for-the-badge" alt="Versão 2.1.9">
  <img src="https://img.shields.io/badge/Linguagem-Python-blue?style=for-the-badge" alt="Python">
  <img src="https://img.shields.io/badge/Finalidade-Educacional-orange?style=for-the-badge" alt="Educacional">
</p>
<p align="center">
  <a href="https://gitlab.com/KasRoudra"><img src="https://img.shields.io/badge/Autor-KasRoudra-purple?style=flat-square" alt="Autor KasRoudra"></a>
  <img src="https://img.shields.io/badge/Código_Aberto-Sim-cyan?style=flat-square" alt="Código aberto">
  <img src="https://img.shields.io/badge/Origem-Bangladesh-green?style=flat-square" alt="Origem Bangladesh">
</p>

---

## 📚 1. Descrição

O **PyPhisher** é uma ferramenta de código aberto desenvolvida em Python para demonstrar técnicas de phishing e engenharia social. Sua documentação descreve páginas de autenticação, servidores web, túneis de rede e mecanismos de registro de informações.

**Esta adaptação destina-se exclusivamente a fins estudantis, pesquisas acadêmicas, auditorias autorizadas e atividades educacionais de Segurança da Informação.** O objetivo é compreender ameaças digitais e desenvolver estratégias de prevenção.

> [!IMPORTANT]
> Use somente em ambientes controlados, com autorização expressa. A finalidade educacional não autoriza obter credenciais reais ou enganar terceiros.

### Continuidade do projeto

Segundo a documentação original, o desenvolvimento passou a integrar o projeto [MaxPhisher](https://gitlab.com/KasRoudra/MaxPhisher). A situação atual de manutenção deve ser conferida nos repositórios oficiais.

---

## 🎯 2. Objetivos educacionais

- Compreender ataques de phishing e engenharia social.
- Identificar páginas falsas e tentativas de fraude.
- Analisar códigos Python, PHP, HTML e JavaScript.
- Estudar autenticação, proteção de credenciais e mecanismos OTP.
- Compreender servidores web, endereçamento e túneis de rede.
- Desenvolver estratégias de defesa e conscientização digital.
- Aplicar princípios éticos e legais em segurança cibernética.

---

## ⚙️ 3. Características do projeto

Conforme a documentação original, o projeto apresenta:

- Interface pelo terminal e suporte a parâmetros de execução.
- Modelos de páginas web e simulações de autenticação.
- Recursos de tunelamento e redirecionamento.
- Modelos relacionados a autenticação OTP.
- Manipulação e pré-visualização de URLs.
- Registro de informações de acesso e análise de erros.
- Distribuição por repositório Git, pacote Python e Docker.

> [!WARNING]
> Esses recursos devem ser estudados apenas em laboratórios próprios ou autorizados, sem coleta de senhas reais nem exposição de páginas enganosas ao público.

---

## 💻 4. Requisitos técnicos

**Linguagem:** Python 3.

**Bibliotecas mencionadas:** `requests`, `rich`, `beautifulsoup4`.

**Componentes:** Git, PHP, SSH e ambiente Linux ou máquina virtual. A documentação original menciona aproximadamente 900 MB de armazenamento.

| Sistema | Compatibilidade informada originalmente |
|---|---|
| Linux | Excelente |
| Android / Termux | Excelente |
| macOS | Experimental |
| iOS | Experimental |
| Windows | Via máquina virtual ou Docker |
| BSD | Não testado |

A compatibilidade não foi verificada independentemente para versões atuais.

---

## 🛠️ 5. Instalação e execução em laboratório

### 5.1. Instalar dependências

**Debian, Ubuntu, Kali Linux e Parrot OS:**

```bash
sudo apt update
sudo apt install git python3 python3-pip php openssh-client -y
```

**Arch Linux e Manjaro:**

```bash
sudo pacman -S git python python-pip php openssh --noconfirm
```

**Fedora e distribuições Red Hat:**

```bash
sudo dnf install git python3 python3-pip php openssh-clients -y
```

**Android — Termux:**

```bash
pkg update && pkg upgrade -y
pkg install git python php openssh -y
```

> [!NOTE]
> Nomes de pacotes e dependências podem variar conforme o sistema e a versão.

### 5.2. Clonar o repositório

**Projeto original:**

```bash
git clone https://gitlab.com/KasRoudra/PyPhisher.git
```

**Repositório de referência da adaptação:**

```bash
git clone https://github.com/profjvidal/PyPhisher.git
```

Escolha apenas um repositório.

### 5.3. Acessar a pasta

```bash
cd PyPhisher
ls -la
```

### 5.4. Conferir as dependências

```bash
cat files/requirements.txt
```

### 5.5. Criar ambiente virtual Python

```bash
python3 -m venv .venv
source .venv/bin/activate
```

No Debian e no Ubuntu pode ser necessário instalar `python3-venv`. A disponibilidade de `venv` no Termux pode variar.

### 5.6. Instalar módulos Python

Após inspecionar o arquivo de dependências:

```bash
python3 -m pip install -r files/requirements.txt
```

O ambiente virtual é preferível à utilização de `--break-system-packages`, pois reduz o risco de alterar o Python gerenciado pelo sistema.

### 5.7. Verificar a sintaxe sem executar

```bash
python3 - <<'PY'
import ast
from pathlib import Path

arquivo = Path('pyphisher.py')
ast.parse(arquivo.read_text(encoding='utf-8'))
print('Análise sintática concluída.')
PY
```

Essa verificação não garante a segurança do código.

### 5.8. Executar a ferramenta

O comando convencional documentado para iniciar o programa é:

```bash
python3 pyphisher.py
```

> [!CAUTION]
> A execução deve ocorrer somente em laboratório isolado e autorizado. Não configure páginas para enganar terceiros, capturar credenciais reais ou receber acessos públicos não autorizados.

### 5.9. Obtenção direta do script

A documentação original também apresenta uma alternativa que combina download e execução imediata. Para permitir a revisão do arquivo, faça o download separadamente:

```bash
wget https://gitlab.com/KasRoudra/PyPhisher/-/raw/main/pyphisher.py
```

Inspecione o arquivo antes de qualquer execução:

```bash
less pyphisher.py
```

Evite executar automaticamente arquivos recém-baixados sem verificar sua procedência, dependências e comportamento.

### 5.10. Pip

A documentação original menciona a distribuição pelo gerenciador Pip. Consulte primeiro as versões disponíveis:

```bash
python3 -m pip index versions pyphisher
```

Antes de instalar, confirme a autoria, a licença e as dependências do pacote.

### 5.11. Docker

A documentação original cita a imagem `kasroudra/pyphisher`. Para consultar seu manifesto, caso esteja disponível:

```bash
docker manifest inspect kasroudra/pyphisher
```

A disponibilidade e a integridade da imagem devem ser verificadas antes de utilizá-la. Um contêiner não substitui o isolamento e as autorizações exigidas pelo laboratório.

---

## 🔐 6. Ambiente de laboratório

1. Utilize máquinas virtuais e redes isoladas.
2. Trabalhe com páginas demonstrativas próprias.
3. Use apenas usuários, senhas e dados fictícios.
4. Não exponha páginas simuladas à Internet pública.
5. Não utilize contas reais de terceiros.
6. Registre a autorização e o escopo das atividades.
7. Analise o tráfego de rede em ambiente controlado.
8. Elimine os dados de teste após as atividades.

---

## 🧪 7. Aplicações educacionais

**Redes de Computadores:** protocolos HTTP/HTTPS, IP, portas, servidores web e tunelamento.

**Segurança da Informação:** autenticação, engenharia social, proteção de credenciais e prevenção de fraudes.

**Programação:** leitura e análise de códigos Python, PHP, HTML e JavaScript.

**Cibersegurança:** análise estática, identificação de comportamentos suspeitos e investigação de páginas fraudulentas.

**Ética e legislação digital:** autorização, privacidade e responsabilidade profissional.

---

## ⚖️ 8. Legislação brasileira aplicável

### Lei nº 12.737/2012 — Lei Carolina Dieckmann

Introduziu disposições sobre delitos informáticos no Código Penal, incluindo o artigo 154-A, relativo à invasão de dispositivo informático.

[Fonte oficial](https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2012/lei/l12737.htm)

### Lei nº 14.155/2021

Alterou dispositivos penais relativos à invasão de dispositivo informático, furto mediante fraude e estelionato eletrônico.

[Fonte oficial](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2021/lei/l14155.htm)

### Lei nº 12.965/2014 — Marco Civil da Internet

Estabelece princípios, garantias, direitos e deveres para o uso da Internet no Brasil.

[Fonte oficial](https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/lei/l12965.htm)

### Lei nº 13.709/2018 — LGPD

Estabelece regras para o tratamento de dados pessoais, inclusive em meios digitais.

[Fonte oficial](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm)

### Decreto-Lei nº 2.848/1940 — Código Penal

Dependendo das circunstâncias, podem ser relevantes o **artigo 154-A** (invasão de dispositivo informático) e o **artigo 171** (estelionato, incluindo fraude eletrônica). A tipificação depende dos fatos e dos requisitos legais.

[Fonte oficial](https://www.planalto.gov.br/ccivil_03/decreto-lei/del2848compilado.htm)

> [!WARNING]
> A finalidade educacional não autoriza automaticamente acessar sistemas, coletar credenciais ou tratar dados pessoais. Condutas sem autorização podem gerar responsabilidade civil e criminal.

---

## 📋 9. Termo de responsabilidade e uso ético

1. **Autorização:** realize testes somente em sistemas próprios ou expressamente autorizados.
2. **Privacidade:** respeite os direitos dos titulares de dados pessoais.
3. **Legalidade:** cumpra as leis e normas institucionais aplicáveis.
4. **Ética:** não utilize o projeto para fraudes ou obtenção indevida de informações.
5. **Segurança:** mantenha as atividades restritas a ambientes controlados.
6. **Responsabilidade:** documente os procedimentos e evite impactos sobre terceiros.

No contexto educacional desta adaptação, não se admite o uso para roubo de senhas, falsificação de identidade, invasões ou outras atividades ilícitas.

---

## 👨‍💻 10. Créditos e reconhecimento

### Desenvolvedor original

**KasRoudra**

- [GitLab](https://gitlab.com/KasRoudra)
- [GitHub](https://github.com/KasRoudra)
- [PyPhisher](https://gitlab.com/KasRoudra/PyPhisher)
- [MaxPhisher](https://gitlab.com/KasRoudra/MaxPhisher)

### Repositório de referência

[profjvidal/PyPhisher](https://github.com/profjvidal/PyPhisher)

### Reconhecimento de autoria

Os direitos autorais e créditos de desenvolvimento pertencem aos respectivos autores. Esta adaptação organiza a documentação em português brasileiro para fins acadêmicos, sem reivindicar autoria sobre o código-fonte original nem vínculo com seu desenvolvedor.

Modificações e redistribuições devem respeitar a licença original e os avisos de direitos autorais aplicáveis.

---

## ⚠️ 11. Aviso legal

**ESTE REPOSITÓRIO DESTINA-SE EXCLUSIVAMENTE A FINS EDUCACIONAIS E DE PESQUISA EM SEGURANÇA DA INFORMAÇÃO.**

O material busca contribuir para a compreensão de ameaças digitais, identificação de vulnerabilidades e desenvolvimento de estratégias defensivas. A disponibilização do código não representa autorização para invasões, fraudes eletrônicas, captura indevida de credenciais ou violação de privacidade.

As responsabilidades decorrentes da utilização do software serão apuradas conforme a legislação aplicável. Este aviso não afasta responsabilidades legalmente atribuíveis a qualquer envolvido.

---

## 📚 12. Referências complementares

- [CERT.br](https://www.cert.br/)
- [Cartilha de Segurança para Internet](https://cartilha.cert.br/)
- [OWASP](https://owasp.org/)
- [NIC.br](https://www.nic.br/)
- [Documentação oficial do Python](https://docs.python.org/3/)
- [Legislação brasileira — Planalto](https://www.planalto.gov.br/)

---

<p align="center"><strong>Segurança da Informação • Redes de Computadores • Cibersegurança • Educação Digital</strong></p>
<p align="center"><em>Conhecer as ameaças digitais é essencial para desenvolver estratégias de prevenção e proteção.</em></p>
