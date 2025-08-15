Documentação do Bot de Música

1. Visão Geral do Projeto
Este documento descreve os requisitos e funcionalidades de um bot de música para a plataforma Discord. O objetivo é criar uma aplicação robusta e funcional em Java, capaz de reproduzir áudio de múltiplas fontes, gerenciar filas de reprodução e oferecer uma experiência de usuário intuitiva.

2. Requisitos Funcionais
  RF1: Reprodução de Áudio
    RF1.1: O bot deve ser capaz de se conectar a um canal de voz.
    RF1.2: O bot deve reproduzir áudio a partir de um link fornecido pelo usuário.
    RF1.3: O bot deve suportar a reprodução de mídias de plataformas como YouTube e Spotify.
  RF2: Gerenciamento de Fila
    RF2.1: O bot deve adicionar a música solicitada à fila de reprodução.
    RF2.2: O bot deve automaticamente passar para a próxima música da fila ao término da atual.
    RF2.3: O bot deve exibir a lista de músicas na fila de reprodução mediante solicitação.
  RF3: Comandos de Controle
    RF3.1: O bot deve processar comandos de texto para controlar a reprodução, incluindo play, pause, resume, skip, stop, queue e volume.
    RF3.2: O bot deve fornecer mensagens de feedback sobre o status da execução de cada comando.
   RF4: Interface de Usuário Interativa
    RF4.1: O bot deve exibir uma interface interativa no chat com botões de controle de reprodução.
    RF4.2: A interface deve incluir botões para Reproduzir/Pausar, Próxima Música, Loop e Desligar.
  RF5: Personalização do Prefixo de Comando
    RF5.1: O bot deve permitir que o prefixo de comando seja alterado por um usuário com as permissões adequadas.

3. Requisitos Não Funcionais

  RNF1: Usabilidade
    RNF1.1: A interface do bot deve ser clara e fácil de usar.
    RNF1.2: O bot deve fornecer mensagens de erro e de status claras para o usuário.

RNF2: Confiabilidade e Estabilidade
    RNF2.1: O bot deve lidar graciosamente com falhas na conexão com as fontes de áudio ou com a plataforma Discord.
    RNF2.2: O áudio deve ser transmitido de forma consistente e sem interrupções.
RNF3: Desempenho
    RNF3.1: O tempo de resposta aos comandos deve ser minimizado para garantir uma boa experiência do usuário.

4. Regras de Negócio
  RN1: Permissões de Acesso
    RN1.1: Apenas usuários com permissão de "Gerenciar Canais" podem alterar o prefixo de comando.
    RN1.2: Comandos de controle de reprodução, como skip e stop, só podem ser executados por usuários que estejam no mesmo canal de voz que o bot.
  RN2: Gerenciamento de Ociosidade
    RN2.1: Se a fila de reprodução estiver vazia por um período superior a 5 minutos, o bot deve se desconectar do canal de voz automaticamente.
  RN3: Limite da Fila
    RN3.1: A fila de reprodução deve ter um limite máximo de 200 músicas para evitar sobrecarga do sistema.

   
