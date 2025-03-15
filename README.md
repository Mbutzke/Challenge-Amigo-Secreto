# Projeto Amigo Secreto - ONE G8 - ALURA

Bem-vindo ao **Amigo Secreto**! 🎁 Este é um projetinho simples e divertido para ajudar na brincadeira clássica de fim de ano (ou qualquer outra ocasião que envolva sorteios entre amigos), proposto pela equipe.

---
## 💡 O que esse projeto faz?
✅ **Adiciona amigos** a uma lista de participantes.  
✅ **Mostra os nomes adicionados** para não esquecer ninguém.  
✅ **Sorteia aleatoriamente** um amigo secreto para cada participante.  
✅ **Exibe o resultado** de forma clara e rápida.

---
## 🚀 Tecnologias Utilizadas

- ``HTML - Estrutura do site. ``
- ``CSS - Estilização e cores.``  
- ``JavaScript - Lógica do sorteio e manipulação da página.``

---
## 🎯 Como Usar?
1️⃣ **Baixe os arquivos** ou clone este repositório.  
2️⃣ **Abra o arquivo `index.html`** no navegador.  
3️⃣ **Adicione os nomes** clicando no botão "Adicionar".  
4️⃣ **Clique em "Sortear amigo"** e veja a mágica acontecer. 🎩✨

---
## 📂 Estrutura do Projeto
📁 **amigo-secreto**  
├── 📄 `index.html`  
├── 📄 `style.css`  
├── 📄 `app.js`  
└── 📁 `assets`  

---
## ✨ Código Principal

### Adicionar Amigo
```javascript
function adicionarAmigo() {
    let input = document.getElementById("amigo");
    let nome = input.value.trim();

    if (nome === "") {
        alert("Por favor, insira um nome.");
        return;
    }

    listaAmigos.push(nome);
    input.value = "";
    atualizarLista();
}
```

### Sortear Amigo
```javascript
function sortearAmigo() {
    if (listaAmigos.length === 0) {
        alert("A lista de amigos está vazia. Adicione pelo menos um nome antes de sortear.");
        return;
    }
    
    let indiceSorteado = Math.floor(Math.random() * listaAmigos.length);
    let amigoSorteado = listaAmigos[indiceSorteado];
    
    let resultado = document.getElementById("resultado");
    resultado.innerHTML = `<li>${amigoSorteado}</li>`;
}
```

---
## 👥 Autor
📌 **Matheus Butzke Silva** - Criador e desenvolvedor.  
| [<img loading="lazy" src="https://media.licdn.com/dms/image/v2/D5603AQGWPB1stocO5g/profile-displayphoto-shrink_800_800/B56ZWFxAVtGUAo-/0/1741705971884?e=1747267200&v=beta&t=IcA0BQom6ATs-qjL_qGugXyGNjaJWr2erpRumnc2sR0" width=115><br><sub>Matheus Butzke Silva</sub>](https://github.com/Mbutzke) |
| :---: |

Este projeto é apenas para fins de aprendizagem logo ele é **open-source**! Sinta-se à vontade para modificar e personalizar do seu jeito. 🚀

