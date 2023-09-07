# 🐙 𝗚𝗶𝘁 .
Comandos Git comumente usados:

## Comandos Básicos:

1. `git init`: Inicializa um novo repositório Git vazio no diretório atual.

2. `git clone <url_do_repositorio>`: Clona um repositório Git existente para o diretório local.

3. `git status`: Exibe o status atual do repositório, mostrando as alterações pendentes, arquivos adicionados, etc.

4. `git add <nome_do_arquivo>`: Adiciona um arquivo específico ao índice (staging area) para ser preparado para um commit.

5. `git add .` ou `git add --all`: Adiciona todos os arquivos modificados e novos ao índice.

6. `git commit -m "Mensagem do commit"`: Cria um novo commit com as alterações adicionadas ao índice, juntamente com uma mensagem descritiva.

7. `git log`: Exibe o histórico de commits do ramo atual, mostrando os autores, datas e mensagens dos commits.

## Ramificação (Branching) e Mesclagem (Merging):

8. `git branch`: Lista todas as branches existentes no repositório.

9. `git branch <nome_da_branch>`: Cria uma nova branch com o nome especificado.

10. `git checkout <nome_da_branch>`: Muda para a branch especificada.

11. `git merge <nome_da_branch>`: Mescla a branch especificada com a branch atual.

12. `git branch -d <nome_da_branch>`: Exclui a branch especificada.

## Atualização e Sincronização:

13. `git pull origin <nome_da_branch>`: Obtém e mescla as alterações mais recentes de um repositório remoto para a branch atual.

14. `git push origin <nome_da_branch>`: Envia os commits locais para um repositório remoto na branch especificada.

## Trabalhando com Tags:

15. `git tag`: Lista todas as tags existentes no repositório.

16. `git tag -a <nome_da_tag> -m "Mensagem da tag"`: Cria uma nova tag anotada com o nome e a mensagem especificados.

17. `git show <nome_da_tag>`: Exibe informações sobre a tag especificada.

18. `git tag -d <nome_da_tag>`: Exclui a tag especificada.

## Desfazendo Alterações:

19. `git checkout -- <nome_do_arquivo>`: Desfaz as alterações não confirmadas em um arquivo específico.

20. `git reset HEAD <nome_do_arquivo>`: Remove um arquivo específico do índice (staging area), mantendo as alterações no diretório de trabalho.

21. `git reset HEAD~<número_de_commits>`: Desfaz um número específico de commits, mantendo as alterações no diretório de trabalho.

22. `git revert <hash_do_commit>`: Cria um novo commit que desfaz as alterações introduzidas por um commit específico.

## Trabalhando com Repositórios Remotos:

23. `git remote add <nome_remoto> <url_do_repositorio>`: Adiciona um novo repositório remoto com o nome especificado e a URL fornecida.

24. `git remote -v`: Lista todos os repositórios.

27. `git remote remove <nome_remoto>`: Remove um repositório remoto com o nome especificado.

26. `git fetch <nome_remoto>`: Busca todas as branches e tags do repositório remoto especificado.

27. `git push <nome_remoto> <nome_branch>`: Envia os commits locais para o repositório remoto na branch especificada.

28. `git push --tags`: Envia todas as tags locais para o repositório remoto.

29. `git pull <nome_remoto> <nome_branch>`: Obtém e mescla as alterações mais recentes do repositório remoto para a branch local especificada.

## Gerenciando Branches Remotas:

30. `git branch -r`: Lista todas as branches remotas disponíveis.

31. `git branch -a`: Lista todas as branches locais e remotas disponíveis.

32. `git checkout -b <nome_da_branch> <nome_remoto>/<nome_da_branch>`: Cria uma nova branch local a partir da branch remota especificada.

33. `git push --set-upstream <nome_remoto> <nome_branch>`: Define a branch local atual como a upstream da branch remota correspondente.

34. `git branch -d -r <nome_remoto>/<nome_da_branch>`: Remove a referência da branch remota especificada.

## Trabalhando com Submódulos:

35. `git submodule add <url_do_repositorio> <caminho_local>`: Adiciona um submódulo ao repositório atual.

36. `git submodule init`: Inicializa os submódulos presentes no repositório.

37. `git submodule update`: Atualiza os submódulos para as versões registradas.

38. `git submodule foreach <comando>`: Executa um comando em cada submódulo.

## Ignorando Arquivos e Diretórios:

39. `.gitignore`: Arquivo onde você especifica padrões de arquivos e diretórios a serem ignorados pelo Git.

40. `git rm --cached <nome_do_arquivo>`: Remove um arquivo do índice, parando de rastreá-lo sem excluí-lo do sistema de arquivos.

41. `git ls-files --others --ignored --exclude-standard`: Lista todos os arquivos não rastreados e ignorados pelo Git.

## Git Stash:

42. `git stash`: Salva as alterações não confirmadas em uma área de stash temporária.

43. `git stash list`: Lista todas as stashs existentes.

44. `git stash apply`: Aplica a stash mais recente, sem removê-la.

45. `git stash pop`: Aplica e remove a stash mais recente.

46. `git stash drop`: Remove a stash mais recente.

47. `git stash branch <nome_branch>`: Cria uma nova branch a partir de uma stash específica.
48. `git stash clear`: Remove todas as stashs existentes.

49. `git stash save "<mensagem>"`: Salva as alterações não confirmadas em uma área de stash temporária, adicionando uma mensagem descritiva.

50. `git stash show`: Exibe as alterações contidas na stash mais recente.

51. `git stash show -p`: Exibe as alterações contidas na stash mais recente no formato de patch.

52. `git stash drop <stash>`: Remove uma stash específica pelo seu índice.

53. `git stash branch <nome_branch> <stash>`: Cria uma nova branch a partir de uma stash específica e a aplica automaticamente, removendo-a em seguida.

54. `git stash apply <stash>`: Aplica uma stash específica sem removê-la da lista de stashs.

55. `git stash pop <stash>`: Aplica e remove uma stash específica da lista de stashs.

56. `git stash branch --track <nome_branch> <stash>`: Cria uma nova branch a partir de uma stash específica, definindo-a como a upstream da branch remota correspondente.

Esses são apenas alguns dos comandos Git mais comumente usados. O Git possui uma ampla gama de recursos e comandos adicionais que podem ser explorados. O Git é um sistema de controle de versão amplamente utilizado na área de desenvolvimento de software. Ele foi criado por Linus Torvalds em 2005 e se tornou uma ferramenta essencial para colaboração em projetos de programação. Ele oferece um ambiente seguro, escalável e eficiente para controlar e gerenciar projetos de software, promovendo a colaboração e melhorando a produtividade dos desenvolvedores.
