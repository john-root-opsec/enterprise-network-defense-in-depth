# 🛡️ Enterprise Defense-in-Depth Network Architecture

<p align="center">
  <strong>Corporate Network Infrastructure & Cybersecurity</strong><br>
  <em>Cisco Packet Tracer · Network Security · Infrastructure Design</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Cisco%20Packet%20Tracer-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco Packet Tracer">
  <img src="https://img.shields.io/badge/Focus-Network%20Security-CC0000?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Network Security">
  <img src="https://img.shields.io/badge/Architecture-Defense--in--Depth-2F855A?style=for-the-badge" alt="Defense in Depth">
</p>

<p align="center">
  <a href="#-english">🇺🇸 English</a> &nbsp;·&nbsp;
  <a href="#-português">🇧🇷 Português</a>
</p>

---

## 📌 Project Overview

An enterprise network infrastructure and cybersecurity simulation developed in **Cisco Packet Tracer**.

The project explores the **Defense-in-Depth** security model through network segmentation, controlled inter-VLAN communication, perimeter security, secure administrative access, and centralized authentication.

> **Objective:** Design a segmented corporate network with layered security controls, simulating real-world enterprise infrastructure.

---

# 🇺🇸 English

## 🏗️ Network Architecture

| Component | Role |
|---|---|
| **Core Layer — Cisco 3560** | Layer 3 switching, inter-VLAN routing, and centralized access policies |
| **Access Layer — Cisco 2960** | Departmental connectivity and VLAN segmentation |
| **Border Router — Cisco 2911** | WAN routing, static routes, and NAT/PAT |
| **Cloud-PT** | Simulated ISP and external network connectivity |
| **Data Center** | Centralized network services and application servers |

## 🔐 Security Implementation

### 01 · Network Segmentation
Dedicated VLANs and IP subnets for IT, Finance, Human Resources, Operations, and the Data Center, reducing unnecessary communication between departments.

### 02 · DMZ & Access Control
A proposed or implemented isolated network segment for public-facing services, protected by **Access Control Lists (ACLs)** to restrict traffic and reduce lateral movement.

### 03 · Centralized AAA / RADIUS
Centralized authentication for administrative access to network devices using a RADIUS server, including fallback authentication policies where configured.

### 04 · Secure Device Management
Secure administrative access using **SSH version 2**, encrypted password configuration, and login warning banners. Telnet is disabled where hardening has been completed.

### 05 · NAT / PAT at the Network Edge
Address translation on the border router to allow internal hosts to access an external network through a shared public-facing address, subject to the simulated WAN configuration.

## 🖥️ Data Center Services

| Server | Purpose |
|---|---|
| `SRV-DHCP-DNS` | Dynamic IP addressing and name resolution |
| `SRV-FTP-FILES` | File transfer services |
| `SRV-WEB` | Internal web services |
| `SRV-EMAIL` | Email services |
| `SRV-APP` | Internal application portal |

## 🎯 Project Goals

- Apply enterprise network design principles.
- Implement VLAN segmentation and inter-VLAN routing.
- Configure centralized network services.
- Strengthen administrative access security.
- Practice ACLs, AAA/RADIUS, and NAT/PAT.
- Validate connectivity and security policies through practical testing.

---

# 🇧🇷 Português

## 📌 Visão Geral do Projeto

Simulação de infraestrutura de redes corporativas e cibersegurança desenvolvida no **Cisco Packet Tracer**.

O projeto explora o conceito de **Defesa em Profundidade (Defense-in-Depth)** por meio da segmentação da rede, do controle da comunicação entre VLANs, da segurança de borda, do acesso administrativo seguro e da autenticação centralizada.

> **Objetivo:** Projetar uma rede corporativa segmentada, com camadas de proteção inspiradas em ambientes empresariais reais.

## 🏗️ Arquitetura da Rede

| Componente | Função |
|---|---|
| **Core Layer — Cisco 3560** | Switching Layer 3, roteamento entre VLANs e políticas de acesso centralizadas |
| **Camada de Acesso — Cisco 2960** | Conectividade dos departamentos e segmentação por VLANs |
| **Roteador de Borda — Cisco 2911** | Roteamento WAN, rotas estáticas e NAT/PAT |
| **Cloud-PT** | Simulação de provedor de Internet e conectividade externa |
| **Data Center** | Centralização de serviços de rede e servidores de aplicações |

## 🔐 Implementação de Segurança

### 01 · Segmentação de Rede
VLANs e sub-redes dedicadas para TI, Financeiro, RH, Operacional e Data Center, reduzindo comunicações desnecessárias entre departamentos.

### 02 · DMZ e Controle de Acesso
Segmento isolado para serviços que precisam de exposição externa, protegido por **ACLs (Listas de Controle de Acesso)** para restringir tráfego e reduzir movimentações laterais.

### 03 · AAA / RADIUS Centralizado
Autenticação centralizada para acesso administrativo aos dispositivos de rede por meio de um servidor RADIUS, com autenticação alternativa quando configurada.

### 04 · Acesso Seguro aos Dispositivos
Gerenciamento administrativo por **SSH versão 2**, configuração de senhas criptografadas e banners de aviso. O Telnet é desativado nos dispositivos em que o hardening foi concluído.

### 05 · NAT / PAT na Borda
Tradução de endereços no roteador de borda para permitir que dispositivos internos acessem uma rede externa utilizando um endereço compartilhado, conforme a configuração da WAN simulada.

## 🖥️ Serviços do Data Center

| Servidor | Finalidade |
|---|---|
| `SRV-DHCP-DNS` | Distribuição automática de IPs e resolução de nomes |
| `SRV-FTP-FILES` | Transferência de arquivos |
| `SRV-WEB` | Serviços web internos |
| `SRV-EMAIL` | Serviços de e-mail |
| `SRV-APP` | Portal interno de aplicações |

## 🎯 Objetivos do Projeto

- Aplicar princípios de arquitetura de redes corporativas.
- Implementar segmentação por VLANs e roteamento inter-VLAN.
- Configurar serviços centralizados de rede.
- Reforçar a segurança do acesso administrativo.
- Praticar ACLs, AAA/RADIUS e NAT/PAT.
- Validar conectividade e políticas de segurança por meio de testes práticos.

---

## ⚠️ Implementation Note

This README describes the intended architecture and security objectives. Features such as DMZ isolation, ACL enforcement, AAA/RADIUS, SSH hardening, and NAT/PAT should be listed as implemented only after they have been configured and tested in the Packet Tracer project.

**Nota de implementação:** Este README descreve a arquitetura planejada e seus objetivos de segurança. Recursos como isolamento de DMZ, ACLs, AAA/RADIUS, hardening SSH e NAT/PAT devem ser apresentados como implementados somente após serem configurados e testados no projeto.
