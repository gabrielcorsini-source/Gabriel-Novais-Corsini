***Aluno***
RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
- ***Metodos***
  - realizarPagamento()
  - agendarAula()
  - cancelarAgendamento()
  - visualizarPlano()
  - receberNotificacao()
  
***Plano***
RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
- ***Metodos***
  - ativar()
  - desativar()
  - alterarPlano()
  - calcularValorTotal()

***Pagamento***
RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
- ***Metodos***
  - processar()
  - cancelar()
  - gerarRecibo()

***Acesso***
RF05, RF09
- idAcesso
- dataHora
- autorizado
- ***Metodos***
  - registrarAcesso()
  - negar()
  - autorizar()

***Aula***
RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima
- ***Metodos***
  - verificarDisponibilidade()
  - agendarAula()
  - removerAgenda()
  
***Agendamento***
RF06, RF10
- idAgendamento
- dataReserva
- status
- ***Metodos***
  - confirmar()
  - cancelar()
  
***Presenca***
RF07
- idPresenca
- data
- presente
- ***Metodos***
  - registrarPresenca()
 
***AvaliacaoFisica***
RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
- ***Metodos***
  - calcularIMC()
  - gerarRelatorio()

***Notificacao***
RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
- ***Metodos***
  - enviar()
  - marcarComoLida()
  
***Classe: Instrutor***
RF07, RF08
- idInstrutor
- nome
- especialidade
- ***Metodos***
  - ministrarAula()
  - avaliarAluno()
    
***Recepcionista***
RF01, RF03
- idRecepcionista
- nome
- ***Metodos***
  - realizarCheckin()
  - cadastrarAluno()

***Gerente***
RF02, RF09
- idGerente
- nome
- ***Metodos***
  - gerarRelatorioFinanceiro()
  - gerenciarFuncionarios()
