# 📧 Email Service - Uber Challenge

> Serviço de envio de e-mails desenvolvido com **Spring Boot** e **Java**, integrado ao **Amazon SES (Simple Email Service)** para envio escalável e confiável de notificações transacionais.

![Java](https://img.shields.io/badge/Java-17-orange?style=flat-square&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-green?style=flat-square&logo=springboot)
![AWS SES](https://img.shields.io/badge/AWS-SES-orange?style=flat-square&logo=amazonses)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

---

## 📋 Índice

- [📖 Sobre o Projeto](#-sobre-o-projeto)
- [✨ Funcionalidades](#-funcionalidades)
- [💻 Tecnologias](#-tecnologias)
- [📋 Pré-requisitos](#-pré-requisitos)

---

## 📖 Sobre o Projeto

Este projeto é um **serviço de e-mail** desenvolvido com **Spring Boot**, criado como parte de um desafio técnico inspirado na arquitetura da Uber. Implementa envio de e-mails transacionais utilizando **Amazon SES**, com arquitetura hexagonal, validação de dados e tratamento robusto de erros.

Ideal para ser consumido por microsserviços que necessitam de notificações por e-mail de forma desacoplada, escalável e cloud-native.

---

## ✨ Funcionalidades

- ✅ **Envio de e-mails via Amazon SES** com suporte a texto plano e HTML
- ✅ **Arquitetura hexagonal** (Ports & Adapters) para desacoplamento e testabilidade
- ✅ **Validação de entrada** com Bean Validation (@Email, @NotNull)
- ✅ **Tratamento de exceções** com `EmailServiceException` e logs estruturados
- ✅ **Configuração externa** de credenciais AWS via variáveis de ambiente
- ✅ **Injeção de dependência** com Spring para fácil manutenção e testes
- ✅ **Pronto para produção** com suporte a retry e monitoramento via CloudWatch

---

## 💻 Tecnologias

| Categoria | Tecnologias |
|-----------|-------------|
| **Linguagem** | Java 17+ |
| **Framework** | Spring Boot 3.x |
| **Cloud** | Amazon SES (Simple Email Service) |
| **AWS SDK** | aws-java-sdk-ses |
| **Arquitetura** | Hexagonal (Ports & Adapters) |
| **Validação** | Bean Validation (Jakarta) |
| **Build** | Maven |
| **Testes** | JUnit 5, Mockito, Spring Boot Test |

---

## 📋 Pré-requisitos

- [Java 17 ou superior](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven 3.8+](https://maven.apache.org/download.cgi)
- Conta AWS com permissões para **Amazon SES**
- E-mail verificado no SES (sandbox ou produção)

---
