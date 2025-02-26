# Principais comandos do Git - Como Usar? 📜

**git clone url-do-repositorio-no-github**
Clona um repositório remoto do GitHub para o seu computador.

**git init**
Inicializa um novo repositório Git no diretório atual. É o primeiro passo para transformar uma pasta comum em um projeto versionado.

**git add .**
Adiciona todos os arquivos e alterações para a área de stage, preparando para o commit.

**git commit -m "mensagem do commit"**
Registra as alterações com uma mensagem descritiva.

**git branch -M main**
Renomeia a branch atual para main.

**git remote add origin https://github.com/usuario/nome-do-repositorio.git**
Adiciona um repositório remoto chamado origin ao seu repositório local.

**git push -u origin main**
Envia os commits da branch main para o repositório remoto e define main como a branch padrão.

**git fetch**
Busca todas as atualizações do repositório remoto sem integrá-las à sua branch.

**git pull origin main**
Atualiza sua branch local com as mudanças do repositório remoto.

**git push --force-with-lease**
Envia alterações locais para o repositório remoto de forma segura, evitando sobrescrever o trabalho alheio.

**git revert id_do_commit_que_vai_ser_revertido**
Desfaz as alterações até um commit específico.

**git reset --hard id_do_commit_anterior_ao_que_vai_ser_apagado**
Redefine o repositório para o estado de um commit específico, apagando tudo que veio depois.

**git commit --amend -m "mensagem_reescrita"**
Altera a mensagem do último commit.

**git cherry-pick HASH_DO_COMMIT**
Pega um commit específico de outra branch e aplica na sua.


## E os Commits Semânticos? 🛠️
Agora que você já sabe o que é o Git, vamos falar sobre Commits Semânticos. Eles são uma forma padronizada de escrever mensagens de commit, usando tipos e descrições que indicam claramente o que foi alterado.
Isso facilita a leitura do histórico, a criação de ferramentas automatizadas e até a geração de changelogs.

Estrutura Básica de um Commit:
```
  <tipo>: <descrição breve>

  [corpo opcional]

  [rodapé opcional]
```

**Tipo**: Indica a natureza da alteração (ex: feat, fix, docs).\
**Descrição**: Uma breve explicação do que foi feito.\
**Corpo**: Detalhes adicionais (opcional).\
**Rodapé**: Informações como revisores ou números de tarefas (opcional).

# Tipos de Commit e Exemplos Práticos 🎯

**feat**: Adiciona uma nova funcionalidade.
Exemplo: git commit -m "✨ feat: Adiciona página de login"

**fix**: Corrige um bug.
Exemplo: git commit -m "🐛 fix: Corrige loop infinito na linha 50"

**docs**: Atualiza a documentação.
Exemplo: git commit -m "📚 docs: Atualiza o README com instruções de instalação"

**test**: Adiciona ou modifica testes.
Exemplo: git commit -m "🧪 test: Adiciona teste para a função de validação de email"

**refactor**: Refatora o código sem mudar a funcionalidade.
Exemplo: git commit -m "♻️ refactor: Substitui funções por arrow functions"

**style**: Ajusta formatação, espaços, linting, etc.
Exemplo: git commit -m "💄 style: Ajusta indentação do arquivo CSS"

**chore**: Atualiza tarefas de build, dependências, etc.
Exemplo: git commit -m "🔧 chore: Adiciona novo pacote ao package.json"

**perf**: Melhora a performance.
Exemplo: git commit -m "⚡ perf: Otimiza tempo de carregamento da API"

**cleanup**: Remove código desnecessário ou comentado.
Exemplo: git commit -m "🧹 cleanup: Remove variáveis não utilizadas"

**remove**: Exclui arquivos ou funcionalidades.
Exemplo: git commit -m "🗑️ remove: Exclui arquivos obsoletos"

**Emojis para Deixar Tudo Mais Visual** 🎨
Você não precisa, mas pode adicionar emojis para tornar seus commits ainda mais visuais. Isso vai de cada profissional e do acordado dentro do projeto.

## Lembre-se!
Seja claro e objetivo na descrição.
Adicione detalhes no corpo do commit, se necessário.
Mantenha a consistência na equipe.

---
# Glossário Git: O Dicionário do Desenvolvedor 📚

## Termos Básicos do Git

1. **Repositório (Repo)**  
   - Um diretório onde seu projeto é armazenado, junto com todo o histórico de alterações.  

2. **Commit**  
   - Um registro das alterações feitas no código em um determinado momento.  

3. **Branch (Ramo)**  
   - Uma linha de desenvolvimento separada, onde você pode trabalhar em novas funcionalidades sem afetar o código principal.  

4. **Merge**  
   - O processo de unir duas branches, combinando as alterações feitas em ambas.  

5. **Pull Request (PR)**  
   - Uma solicitação para integrar as alterações de uma branch em outra (geralmente da sua branch para a `main`).  

6. **Clone**  
   - Copiar um repositório remoto para o seu computador local.  

7. **Fork**  
   - Criar uma cópia independente de um repositório na sua conta do GitHub.  

8. **Push**  
   - Enviar suas alterações locais para um repositório remoto.  

9. **Pull**  
   - Atualizar seu repositório local com as alterações do repositório remoto.  

10. **Fetch**  
    - Buscar as atualizações do repositório remoto sem aplicá-las ao seu código local.  

11. **Staging Area (Área de Stage)**  
    - Uma área temporária onde você prepara as alterações antes de fazer um commit.  

12. **HEAD**  
    - Um ponteiro que indica o commit atual no qual você está trabalhando.  

13. **Tag**  
    - Um marcador usado para identificar um ponto específico no histórico, como uma versão do projeto (ex: v1.0.0).  

14. **Revert**  
    - Desfazer um commit específico, criando um novo commit que cancela as alterações.  

15. **Reset**  
    - Voltar o repositório para um estado anterior, descartando commits ou alterações.  

16. **Cherry-pick**  
    - Aplicar um commit específico de uma branch em outra.  

17. **Conflict (Conflito)**  
    - Quando duas alterações diferentes são feitas na mesma parte do código e o Git não sabe qual versão manter.  

18. **Rebase**  
    - Reorganizar os commits de uma branch para aplicá-los em cima de outra branch.  

19. **Stash**  
    - Guardar temporariamente as alterações que você não quer commitar ainda.  

20. **Origin**  
    - O nome padrão dado ao repositório remoto de onde você clonou o projeto.  

21. **Upstream**  
    - O repositório remoto original de onde você fez um fork.  

22. **Workflow**  
    - O processo ou fluxo de trabalho que sua equipe usa para gerenciar branches, commits e merges.  
