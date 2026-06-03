# Contador de Producao Agricola

Um aplicativo web mobile-first desenvolvido para atuar como um contador digital de producao (tally counter), ideal para safras, colheitas (como a do cafe) e controle de linha de producao. O foco principal do projeto e a ergonomia e a operacao "cega", permitindo que o trabalhador conte itens sem precisar olhar para a tela do dispositivo.

## Funcionalidades Principais

* Contagem Persistente: O numero atual e salvo automaticamente no armazenamento local do navegador (LocalStorage), evitando perda de dados caso a aba seja fechada.
* Feedback Sensorial: Cada contagem emite um bipe sonoro (Web Audio API) e uma vibracao (Vibration API), garantindo ao usuario que o item foi contabilizado com sucesso.
* Contagem por Movimento (Giroscopio): Atraves da integracao com a DeviceOrientation API, o aplicativo permite contabilizar itens apenas inclinando o dispositivo para frente, funcionando como um controle remoto ou gatilho fisico.
* Modo Trava de Seguranca: 
  * Bloqueia o botao de zerar a contagem.
  * Impede navegacao acidental (voltar ou fechar a pagina).
  * Mantem a tela do dispositivo sempre ativa (integracao com a Screen Wake Lock API), ideal para sessoes de trabalho continuas.
* Interface Otimizada: Botoes grandes com alto contraste e prevencao contra selecao de texto ou zoom acidental durante toques rapidos.

## Tecnologias Utilizadas

Este projeto foi construído utilizando tecnologias web nativas (Vanilla Web), sem a necessidade de frameworks externos:

* HTML5 (Estrutura e semantica)
* CSS3 (Responsividade, UI/UX focado em toques rapidos e feedback visual)
* JavaScript ES6+ (Logica de estado e interacao com APIs nativas do navegador)
* APIs do Navegador: Web Audio API, Vibration API, Screen Wake Lock API e Device Orientation API.

## Como Executar o Projeto

Nao ha necessidade de instalacao de dependencias. O aplicativo roda diretamente no navegador.

1. Faca o clone deste repositorio:
   git clone https://github.com/SEU_USUARIO/nome-do-repositorio.git

2. Abra o arquivo index.html no seu navegador.

Aviso Importante sobre o Sensor de Movimento:
Para que o recurso de contagem por inclinacao do aparelho (giroscopio) e o bloqueio de tela (Wake Lock) funcionem perfeitamente em dispositivos moveis (especialmente iOS), e estritamente necessario que o aplicativo seja acessado atraves de uma conexao segura (HTTPS). Recomenda-se hospedar o projeto gratuitamente no GitHub Pages, Vercel ou Netlify.

## Desenvolvedor

Projeto desenvolvido com o objetivo de facilitar o trabalho braçal e o registro de produtividade no campo atraves da tecnologia.
