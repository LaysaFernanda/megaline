# megaline
Projeto de análise de planos pré-pagos de uma empresa de telecomunicações.

Neste projeto analisei o comportamento dos clientes dos planos pré-pagos da empresa de telecomunicações Megaline, para saber quais dos planos dão mais receita para ajustar o orçamento de publicidade.

### Descrição dos dados
A tabela users (dados sobre usuários):
- user_id — identificação do usuário
- first_name — nome do usuário
- last_name — último sobrenome do usuário
- age — idade do usuário (em anos)
- reg_date — data da inscrição (dd, mm, aa)
- churn_date — a data que o usuário parou de usar o serviço (se o valor for ausente, o plano estava sendo usado quando esse dado foi gerado)
- city — cidade de residência do usuário
- plan — nome do plano

A tabela calls (dados sobre as chamadas)
- id — identificador de chamada unívoco
- call_date — data da chamada
- duration — duração da chamada (em minutos)
- user_id — o identificador do usuário que faz a chamada

A tabela messages (dados nas mensagens de texto):
- id — identificador unívoco de mensagem de textos
- message_date — data da mensagem de texto
- user_id — o identificador do usuário que envia a mensagem de texto

A tabela internet (dados sobre sessões web):
- id — identificador de sessão unívoco
- mb_used — o volume de dados gasto durante a sessão ( em megabytes)
- session_date — data da sessão web
- user_id — identificador do usuário

A tabela plans(dados sobre os planos):
- plan_name — o nome do plano de chamadas
- usd_monthly_fee — preço mensal em dólares dos EUA
- minutes_included — pacote de minutos mensal
- messages_included — pacote de mensagens de texto mensal
- mb_per_month_included — pacote de volume de dados (em megabytes)
- usd_per_minute — preço por minuto depois de exceder o limite do pacote (por exemplo, se o pacote inclui 100 minutos, o primeiro minuto excedente será cobrado)
- usd_per_message — preço por mensagem de texto depois de exceder o limite do pacote
- usd_per_gb — preço por gigabyte extra de dados após exceder o limite do pacote (1 GB = 1024 megabytes)

### Bibliotecas usadas
- pandas
- matploylib
- scipy
- seaborn
