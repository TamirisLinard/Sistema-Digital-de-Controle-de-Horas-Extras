# **Sistema Digital de Controle de Horas Extras** :clock3:

**Alunos:** Caio Eduardo Zanotelli, Raul César de Matos, Tamiris Linard

**Turma:** EO1M

**Professora:** Fabiana Bravim de Freitas


## Descrição
O sistema permite que gestores e funcionários façam login, registrem seus pontos diários e acompanhem seus dados de horas trabalhadas.
Com base nesses registros, o programa calcula automaticamente:
- Horas extras de 50% (durante a semana)
- Horas extras de 100% (fins de semana e feriados)
- Valor total das horas extras e o salário final do funcionário


## Sumário
- Estrutura do Código
- Como Compilar e Executar
- Exemplo de Uso
- Constantes Importantes
- Melhorias Futuras

## Funcionalidades
:small_orange_diamond: **Usuários**
 - Cadastro de funcionários e gestores
 - Cada usuário possui:
   - Nome
   -  Matrícula (máximo de 10 dígitos)
   -  Tipo (funcionário/gestor)
   -  Senha
   -  Salário mensal

:small_orange_diamond: **Ponto**
  -  Registro de ponto normal
  -  Registro de hora extra (semana - 50%)
  -  Registro de hora extra (fim de semana - 100%)
  -  Exibição de todos os pontos registrados

:small_orange_diamond: **Relatórios**
  - Relatório de horas extras (por funcionário)
  - Tabela de salário final (salário base + adicionais)
  - Listagem de usuários cadastrados


:small_orange_diamond: **Login**
  - Login individual por matrícula e senha
  - Menu diferenciado para gestor e funcionário


## Estrutura do Código

O código está organizado da seguinte forma:
 - **Cadastro:** Criação de novos usuários
 - **Login:** Verificação de credenciais e acesso
 - **Ponto:** Registro de entrada e saída
 - **Relatórios:** Cálculo e exibição de horas extras e salário final
 - **Menus:** Interface textual interativa para cada tipo de usuário
 - **Funções auxiliares:** Leitura de strings, limpeza de buffer e cálculos de tempo

## Como Compilar e Executar
**Pré-requisitos**
- Compilador GCC (ou equivalente)
- Sistema operacional compatível com C padrão (Windows, Linux, macOS)

**Comandos**
- Compilar o programa
>  gcc main.c -o sistema_ponto

- Executar o programa
> ./sistema_ponto

- No Windows:

> gcc main.c -o sistema_ponto.exe
> sistema_ponto.exe

**Constantes Importantes**

| Constante    | Descrição       | Valores |
| :---         |     :---:      |          ---: |
| MAX_USUARIOS   | Número máximo de usuários     | 100    |
| MAX_PONTOS    | Número máximo de registros de ponto      | 200     |
| JORNADA_MENSAL| Jornada mensal padrão em horas   | 220   |
| ADICIONAL_SEMANA   | Multiplicador para horas extras de 50%      | 1.5     |
| ADICIONAL_FIMSEMANA  | Multiplicador para horas extras de 100%     | 2.0    |
| MAX_MATRICULA_LEN   | Tamanho máximo da matrícula       | 10     |


## Exemplo de Uso

:small_orange_diamond: No menu principal:
  - Cadastrar Usuario
  - Login
  - Sair

:small_orange_diamond: Após o login como funcionário:
  - Bater ponto normal
  - Bater ponto extra (semana - 50%)
  - Bater ponto extra (fim de semana - 100%)
  - Sair da conta

:small_orange_diamond: Como gestor, você tem acesso adicional a:
  - Ver usuarios cadastrados
  - Ver registros de ponto
  - Relatorio de horas extras
  - Tabela de salario final
  - Sair da conta

## Melhorias Futuras
- Salvamento de dados em arquivo (.txt ou .csv)
- Edição e exclusão de usuários e pontos
- Exportação automática de relatórios
- Interface gráfica (GUI)
- Integração com banco de dados
