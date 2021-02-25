# AR_BASIC
 Estrutura base para RA com Unity + Vuforia

Ao editar este projeto no Unity, é necessário alterar a License Key do Vuforia dentro do projeto e adicionar a nova database de imagens selecionadas.
Parte desse processo pode ser feito no próprio site do Vuforia -> Develop (https://developer.vuforia.com/vui/develop/licenses).
==================
A lincese key pode ser obtida na aba License Manager, botão Get Development key. Após registro da nova chave, para alterar a chave atual do projeto, é necessário abri-lo no Unity, selecionar, na Hierarquia, o objeto AR Camera -> Open Vuforia Engine configuration, e colar a chave no campo App License Key.
Obs: Não é necessário clicar no botão Add License, pois ele irá redirecionar para o site do Vuforia, para realizar o processo já descrito aqui.
==================
A database é gerada na aba Target Manager (https://developer.vuforia.com/vui/develop/databases), após criar uma nova base (botão Add Database), o usuário faz o upload de no mínimo uma imagem (Add Target), clica em Download Database(All), e então escolhe a opção Unity Editor como plataforma de desenvolvimento.
==================

Para cada carta presente na database é necessário criar um objeto novo na Hierarquia, do tipo Vuforia -> Image Target.
Nesse novo objeto, na janela do Inspetor, alterar a opção Image Target para a imagem desejada.
Durante a execução da aplicação, cada Image Target só passa a existir quando a imagem associada é identificada pela câmera
