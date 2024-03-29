# Proposta-de-Sistema-Orientado-a-Objetos-

# Sistema Orientado a Objetos

# Link do Figma
https://www.figma.com/file/HJSSCUDIqkR0vkYQwKxbkV/Projeto-Integrador-Senac?type=design&node-id=0%3A1&mode=design&t=E2czg0anMQVIgALB-1

## Descrição dos Casos de Uso

### Caso de Uso: Fazer Login
**Cenário Principal:**
- **Ator:** Aluno, Professor, Fornecedor
- **Pré-condição:** O usuário possui credenciais válidas.
  
**Fluxo Principal:**
1. O usuário acessa a página de login.
2. O sistema exibe campos para inserir nome de usuário e senha.
3. O usuário insere suas credenciais.
4. O sistema verifica as credenciais.
5. O sistema autentica o usuário e permite acesso ao sistema.

**Cenário Alternativo 1 - Credenciais Inválidas:**
- **Fluxo Alternativo:**
  - No passo 4 do cenário principal, se as credenciais forem inválidas:
    - O sistema exibe uma mensagem de erro.
    - O usuário tem a opção de tentar novamente.

**Cenário Alternativo 2 - Conta Bloqueada:**
- **Fluxo Alternativo:**
  - No passo 4 do cenário principal, se a conta estiver bloqueada:
    - O sistema informa ao usuário que a conta está bloqueada por tentativas excessivas.
    - O usuário é orientado a entrar em contato com o suporte técnico.

**Pós-condição:** O usuário está autenticado no sistema e pode acessar as funcionalidades correspondentes ao seu papel (aluno, professor, fornecedor).

### Caso de Uso: Ver Boletim
**Cenário Principal:**
- **Ator:** Aluno
- **Pré-condição:** O aluno está autenticado no sistema.

**Fluxo Principal:**
1. O aluno acessa o menu de boletim.
2. O sistema exibe as notas e resultados das avaliações do aluno.
3. O aluno pode visualizar seu desempenho acadêmico por disciplina.

**Cenário Alternativo 1 - Nenhuma Nota Registrada:**
- **Fluxo Alternativo:**
  - No passo 2 do cenário principal, se não houver notas registradas:
    - O sistema informa ao aluno que não há notas disponíveis ainda.

**Cenário Alternativo 2 - Problemas de Exibição:**
- **Fluxo Alternativo:**
  - No passo 2 do cenário principal, se houver problemas na exibição das notas:
    - O sistema apresenta uma mensagem de erro.
    - O aluno é instruído a entrar em contato com o suporte técnico.

**Pós-condição:** O aluno visualiza suas notas e resultados acadêmicos.

### Caso de Uso: Postar Conteúdos para Suas Turmas
**Cenário Principal:**
- **Ator:** Professor
- **Pré-condição:** O professor está autenticado no sistema.

**Fluxo Principal:**
1. O professor acessa a área de postagem de conteúdos.
2. O sistema permite que o professor selecione a turma.
3. O professor faz upload de arquivos ou adiciona conteúdo para a turma selecionada.
4. O sistema confirma a postagem bem-sucedida.

**Cenário Alternativo 1 - Falha no Upload:**
- **Fluxo Alternativo:**
  - No passo 3 do cenário principal, se houver falha no upload:
    - O sistema exibe uma mensagem de erro.
    - O professor é orientado a tentar novamente ou verificar a conexão.

**Cenário Alternativo 2 - Turma Inexistente:**
- **Fluxo Alternativo:**
  - No passo 2 do cenário principal, se a turma selecionada não existir:
    - O sistema informa ao professor sobre a inexistência da turma selecionada.

**Pós-condição:** O conteúdo é postado com sucesso para a turma selecionada.

### Caso de Uso: Consultar Demanda de Materiais
**Cenário Principal:**
- **Ator:** Fornecedor
- **Pré-condição:** O fornecedor está autenticado no sistema.

**Fluxo Principal:**
1. O fornecedor acessa a área de consulta de demanda de materiais.
2. O sistema exibe uma lista de materiais requisitados pela universidade.
3. O fornecedor revisa a lista de materiais demandados.

**Cenário Alternativo 1 - Lista Vazia:**
- **Fluxo Alternativo:**
  - No passo 2 do cenário principal, se não houver itens na lista de materiais:
    - O sistema informa ao fornecedor que não há demanda de materiais no momento.

**Cenário Alternativo 2 - Problemas de Acesso:**
- **Fluxo Alternativo:**
  - No passo 1 do cenário principal, se houver problemas de acesso:
    - O sistema exibe uma mensagem de erro.
    - O fornecedor é orientado a verificar sua conexão ou entrar em contato com o suporte.

**Pós-condição:** O fornecedor revisa com sucesso a demanda de materiais requisitados.

# Diagrama de Casos de Uso
## Aluno
![image](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/f5435f45-ee1d-49c7-a625-480e6ecd1102)
## Professor
![image](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/531bfe1f-61dc-4a6b-a19a-89bf26182654)
## Fornecedor
![image](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/f56cef32-be71-4ba4-b9d1-74ccd7b62a8b)

# Diagrama de Classes
![image](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/555e3a00-19b6-49f9-86a3-6bed78212d07)

# Interfaces do Projeto
## Entrar e Cadastro
![signIn](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/efdddbf0-ebf0-4244-a8ec-2b3fe614f6c1)
## Aluno
![aluno](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/03fb0b29-b897-4867-b7b8-5a85fa811b83)
## Professor
![professor](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/21d00d86-cf21-4b5d-912f-0d7a5eac922f)
## Fornecedor
![fornecedor](https://github.com/NickBritoDev/Proposta-de-Sistema-Orientado-a-Objetos-/assets/122695407/16cacad2-89b4-437b-b42a-5f62efde05b2)
