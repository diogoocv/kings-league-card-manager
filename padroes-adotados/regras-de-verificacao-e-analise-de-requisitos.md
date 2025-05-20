    # Regras de Verificação e Análise de Requisitos   

## 1. Nomenclatura Padrão  
Tipo    Formato     Exemplo                                                                 

RF      RFXX        `RF01`  - O sistema deve permitir login de usuários do tipo Player e Admin. 
RNF     RNFXX       `RNF01` - O sistema deve ter tempo de resposta inferior a 3s em 90% das requisições. 

## 2. Regras de Especificação  
### 2.1 Atomicidade (Regra 1)  
- Cada requisito deve descrever **uma única funcionalidade ou restrição**.  
- Exemplo inválido:  
    "O sistema deve cadastrar cartas e permitir sua edição por administradores."  
- Exemplo válido:  
    `RF02` - O sistema deve permitir cadastro de novas cartas por administradores.  
    `RF03` - O sistema deve permitir edição de cartas existentes por administradores.  

### 2.2 Rastreabilidade (Regra 2)  
- Todo requisito deve conter:  
    - **ID único** (RFXX/RNFXX)  
    - **Categoria** (ex: "Núcleo do Sistema", "Requisito de Segurança")  
    - Exemplo:  
        `RNF03` - O banco de dados deve ser MySQL 8.x. *(Requisito de Infraestrutura)*  

### 2.3 Verificabilidade (Regra 3)  
- Requisitos devem ser formulados como **critérios de teste objetivos**.  
- Não verificável:  
    "A interface deve ser intuitiva."  
- Verificável:  
    `RNF04` - Usuários devem conseguir abrir uma caixa de cartas em até 3 cliques a partir da tela inicial.  

## 3. Termos Técnicos  
Termo           Definição                                  

Admin           Usuário com permissão para realizar alterações no sistema, como cadastro de cartas e campeonatos. 
Player          Usuário comum que coleta cartas e monta sua equipe. 
Card            Representação digital de um jogador da Kings League. 

