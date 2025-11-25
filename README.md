# Ataques de força bruta com Medusa (laboratório controlado)

> ⚠️ **AVISO IMPORTANTE – USO ÉTICO**
>
> Este repositório documenta **ataques de força bruta e password spraying**
> realizados **exclusivamente em um ambiente de laboratório**:
> - Máquina atacante: Kali Linux
> - Máquina alvo: Metasploitable2 e DVWA
>
> **Nunca** use estas técnicas contra sistemas para os quais você não tem
> autorização explícita. Isso é ilegal e antiético.

---

## Objetivo

Demonstrar, em ambiente controlado, como:

1. Realizar um ataque de força bruta contra o serviço **FTP** da máquina
   Metasploitable2 usando **Medusa**.
2. Realizar um ataque de força bruta contra o formulário de login da
   aplicação web **DVWA**.
3. Realizar um ataque de **password spraying** contra o serviço **SMB**
   após enumeração de usuários com **enum4linux**.

Ao final, são apresentadas recomendações de segurança para mitigar esse
tipo de ataque.

---

## Ambiente de laboratório

- **Virtualização**: VirtualBox / VMware (ou similar)
- **Máquina atacante**: Kali Linux
- **Máquina alvo**: Metasploitable2 (rodando DVWA e serviços FTP/SMB)
- **Rede**: Host-Only ou rede privada interna
- **Exemplo de IP da vítima**: `192.168.56.11` (ajuste conforme seu lab)

---

## Ferramentas utilizadas

- [Medusa](http://www.foofus.net) – ferramenta de força bruta para vários serviços
- `ftp` – cliente FTP em linha de comando
- `enum4linux` – enumeração de serviços SMB
- `smbclient` – cliente SMB
- Navegador web (para acessar DVWA e inspecionar o tráfego de login)

---


