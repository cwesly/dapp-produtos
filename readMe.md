# 🔗 DApp — Registro de Produtos na Blockchain

Aplicação descentralizada (DApp) desenvolvida para a disciplina de **Tópicos Especiais em Computação - Blockchain** do curso de Análise e Desenvolvimento de Sistemas do **IFPI — Campus Parnaíba**.

**Professor:** Denylson Melo

---

## 👥 Grupo 08

| Nome |
|---|
| Cauã Wesly |
| Giovanna |
| Antônio de Gois |
| Francisco Ryan |

---

## 📌 Sobre o Projeto

O projeto resolve um problema real de **rastreabilidade e autenticidade de produtos**. Empresas podem registrar seus produtos na blockchain garantindo que as informações sejam imutáveis, transparentes e verificáveis por qualquer pessoa — sem depender de um servidor central ou de uma autoridade intermediária.

Qualquer tentativa de falsificação ou adulteração de registros é impossível, pois os dados gravados na blockchain não podem ser alterados após o registro.

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| **Solidity** | Linguagem de programação do contrato inteligente |
| **Remix IDE** | Ambiente de desenvolvimento e deploy do contrato |
| **Ethereum / Sepolia** | Blockchain e testnet utilizada |
| **MetaMask** | Carteira digital e assinatura de transações |
| **Ethers.js v5** | Biblioteca de integração entre a interface e a blockchain |
| **HTML / CSS / JavaScript** | Interface web da DApp |

---

## 📁 Estrutura do Projeto

```
dapp-produtos/
├── index.html              # Interface web da DApp
├── RegistroProdutos.sol    # Contrato inteligente em Solidity
└── README.md               # Documentação do projeto
```

---

## 🚀 Contrato na Blockchain

O contrato foi publicado na testnet **Sepolia** e pode ser verificado publicamente:

- **Endereço do contrato:**
  `0x33d21737A14DAC93734C8F9fF78dB8c4cF0Fe986`

- **Verificar no Etherscan:**
  https://sepolia.etherscan.io/address/0x33d21737A14DAC93734C8F9fF78dB8c4cF0Fe986

---

## ⚙️ Funcionalidades

- ✅ Conectar carteira MetaMask
- ✅ Registrar produto na blockchain (nome, descrição, fabricante)
- ✅ Buscar produto pelo ID
- ✅ Visualizar total de produtos registrados
- ✅ Cada registro guarda o endereço de quem registrou
- ✅ Todas as transações verificáveis no Etherscan

---

## 🖥️ Como Rodar o Projeto

### Pré-requisitos

Antes de tudo, instale e configure:

1. **Google Chrome** — https://chrome.google.com
2. **MetaMask** (extensão do Chrome) — https://metamask.io
3. **VS Code** — https://code.visualstudio.com
4. **Extensão Live Server** no VS Code

### Configurar a MetaMask

1. Crie uma conta na MetaMask
2. Clique no nome da rede no topo
3. Ative "Mostrar redes de teste"
4. Selecione a rede **Sepolia**

### Obter ETH de teste

Acesse o faucet e cole o endereço da sua carteira:
https://cloud.google.com/application/web3/faucet/ethereum/sepolia

### Rodar a interface

1. Clone o repositório ou baixe o ZIP
2. Abra a pasta no VS Code
3. Clique com botão direito no `index.html`
4. Clique em **"Open with Live Server"**
5. O Chrome abrirá em `http://127.0.0.1:5500/index.html`
6. Clique em **"Conectar MetaMask"** e comece a usar

---

## 📖 Como o Contrato Funciona

O contrato `RegistroProdutos.sol` possui as seguintes funções:

### `registrarProduto(nome, descricao, fabricante)`
Registra um novo produto na blockchain. Cada produto recebe um ID único, a data do registro e o endereço de quem registrou. Cobra uma pequena taxa em SepoliaETH.

### `buscarProduto(id)`
Retorna todos os dados de um produto pelo ID. Não cobra taxa por ser apenas leitura.

### `produtoExiste(id)`
Verifica se um produto com determinado ID foi registrado.

### `totalProdutos()`
Retorna o número total de produtos registrados no sistema.

---

## 🔍 Por que Blockchain?

| Problema tradicional | Solução com blockchain |
|---|---|
| Banco de dados pode ser adulterado | Registros imutáveis após gravação |
| Empresa central pode manipular dados | Sem intermediários ou autoridade central |
| Difícil rastrear quem fez cada registro | Endereço do registrante gravado permanentemente |
| Sistema pode sair do ar | Rede distribuída em milhares de nós |

---

## 📝 Licença

Projeto acadêmico desenvolvido para fins educacionais — IFPI Campus Parnaíba, 2026.