# ProvaDigital

## 📌 Visão Geral

**ProvaDigital** é um sistema brasileiro de registro forense local criado para preservar evidências do estado de um computador ao longo do tempo. Seu objetivo é permitir que o usuário **prove tecnicamente** que determinados arquivos, programas, serviços ou configurações **não existiam** em um momento anterior.

O foco do ProvaDigital não é bloquear, remover ou acusar. Ele **registra fatos**, cria uma **linha do tempo confiável** e preserva a integridade das informações.

---

## 🎯 Objetivo do Projeto

* Criar um **estado inicial confiável** do sistema
* Monitorar alterações ao longo do tempo
* Registrar eventos de forma **imutável e verificável**
* Permitir comprovação técnica em situações de disputa, auditoria ou análise forense

Em resumo:

> *Se algo apareceu depois, o ProvaDigital consegue provar.*

---

## 🧠 Conceito Central

O ProvaDigital funciona como uma **testemunha técnica automática** do sistema operacional.

Ele responde com precisão a perguntas como:

* Isso existia antes?
* Quando apareceu?
* Onde foi instalado?
* Qual era o estado do sistema antes da alteração?

---

## 🧱 Arquitetura do Sistema

O sistema é dividido em quatro módulos principais:

### 1️⃣ EstadoInicial

Responsável por criar o **snapshot base** do sistema.

Registra:

* Programas instalados
* Arquivos críticos
* Serviços ativos
* Inicialização automática
* Usuários do sistema

Esse snapshot define o **marco zero**.

---

### 2️⃣ Monitoramento

Executa verificações periódicas (ex: a cada 30 segundos) e detecta:

* Novos arquivos
* Novos programas
* Novos serviços
* Alterações em pontos sensíveis

Cada alteração gera um **evento forense**.

---

### 3️⃣ RegistroFiel

Cria logs cronológicos com:

* Data e hora
* Tipo do evento
* Caminho do item
* Hash criptográfico

Os registros são **encadeados**, garantindo integridade.

---

### 4️⃣ ArquivoDeProvas

Organiza e preserva os registros para:

* Auditoria
* Exportação
* Verificação posterior

---

## 📂 Estrutura de Pastas (Padrão)

```
ProvaDigital/
 ├── estado_inicial/
 │    └── snapshot_YYYY-MM-DD_HH-MM.json
 ├── registros/
 │    └── provadigital.log
 ├── hashes/
 │    └── cadeia.hash
 └── config.json
```

---

## 🔐 Integridade e Confiabilidade

O ProvaDigital utiliza:

* Hash criptográfico (SHA-256)
* Encadeamento de registros
* Logs somente de acréscimo (append-only)

Qualquer tentativa de alteração posterior invalida a cadeia de registros.

---

## ⚖️ Linguagem Forense

O sistema evita termos acusatórios.

Utiliza linguagem técnica e neutra:

* "detectado"
* "não constava no estado anterior"
* "registro cronológico"
* "evento observado"

Isso torna os registros mais claros e defensáveis.

---

## 🧪 Exemplo de Evento Registrado

```
[2026-01-30 12:16:30]
EVENTO: Novo arquivo detectado
CAMINHO: C:\Windows\System32\abc.exe
HASH: 91af3c...
OBSERVAÇÃO: Não constava no estado inicial
```

---

## 🛡️ O que o ProvaDigital NÃO faz

* ❌ Não remove arquivos
* ❌ Não bloqueia programas
* ❌ Não acusa usuários
* ❌ Não interfere no sistema

Ele apenas **registra e preserva fatos**.

---

## 📌 Casos de Uso

* Defesa técnica em acusações indevidas
* Auditoria de sistemas
* Análise forense pessoal
* Monitoramento de integridade
* Registro histórico do sistema


---

## 📜 Licença



---

## ✍️ Autor

Projeto idealizado para autodefesa digital e preservação da verdade técnica.


