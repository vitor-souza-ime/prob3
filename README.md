# P-ROB3 - Controle Automatizado de Manipulador Robótico em Webots

Este projeto implementa o **controle automatizado** de um manipulador robótico **P-ROB3** utilizando o simulador [Webots](https://cyberbotics.com/).  
O código `main.c` demonstra a execução de **tarefas de apreensão, transporte e liberação de objetos** (como latas cilíndricas) usando os **sete motores do braço e a garra adaptativa**.

---

## 📌 Funcionalidades
- Controle completo dos **sete graus de liberdade** do P-ROB3.  
- Rotinas para **abrir e fechar a garra** do manipulador.  
- Sequência automatizada de **apreensão, transporte e deposição de objetos**.  
- Controle temporal preciso para operações suaves e coordenadas.  
- Modularidade para futuras extensões, como integração com visão computacional ou planejamento de trajetórias.

---

## 📂 Estrutura do Projeto
- `main.c` → código principal de controle do P-ROB3.  
- **Motores do braço e garra** mapeados para os dispositivos Webots.  

---

## 🚀 Execução no Webots

### Pré-requisitos
- [Webots R2023a ou superior](https://cyberbotics.com/).  
- Compilador C compatível (ex: `gcc`).  

### Passos
1. Clone o repositório:
   
   git clone https://github.com/vitor-souza-ime/prob3.git
   cd prob3

2. Abra o Webots e carregue o mundo que contém o P-ROB3.
3. Compile e execute o `main.c` dentro do Webots.

---

## 📖 Funcionamento

* O braço executa uma sequência pré-programada para pegar um objeto, levantá-lo, rotacionar o braço e depositá-lo em outra posição.
* A **garra** pode ser aberta ou fechada utilizando as funções `open_gripper()` e `close_gripper()`.
* O tempo de cada movimento é controlado pela função `passive_wait()` para garantir suavidade na operação.

---

## 📌 Referências

* CYBERBOTICS LTD. *Webots Documentation*. Disponível em: [https://cyberbotics.com/doc](https://cyberbotics.com/doc).
* F\&P ROBOTICS. *P-ROB 3-48V*. Disponível em: [https://qviro.com/product/f-p-robotics/p-rob-3-48v](https://qviro.com/product/f-p-robotics/p-rob-3-48v).

---

## 📜 Licença

Este projeto está licenciado sob a **Apache License 2.0**, conforme indicado nos comentários do arquivo `main.c`.
