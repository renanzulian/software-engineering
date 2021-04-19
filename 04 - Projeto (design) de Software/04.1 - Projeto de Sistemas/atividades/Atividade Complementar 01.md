# Exercíte o conceito de casos de uso crítico para definição da arquitetura

## Requisitos

**R1**- O sistema deve permitir que os alunos visualizem as notas obtidas nas atividades acadêmicas avaliativas por disciplina e por semestre

**R2**- O sistema deve permitir que os professores lancem notas das atividades acadêmicas avaliativas das disciplinas a quais estão alocados

**R3**- O sistema deve manter informações sobre as disciplinas da grade curricular de cada curso incluindo carga horária, ementa, objetivos e bibliografia

**R4**- O sistema deve permitir ao coordenador a abertura de turmas para as disciplinas, incluindo as salas de aula e laboratórios onde serão ministradas, os horários e dias da semana em que as aulas acontecerão.

**R5**- O sistema deve permitir que os alunos se matriculem nas disciplinas oferecidas em um semestre letivo

**R6**- O sistema deve buscar dados relativos aos professores no Sistema de Recursos Humanos para verificar se estes possuem habilitação para serem alocados em determinada oferta de disciplina.

**R7**- O sistema deve enviar dados relativos à matrícula em disciplinas para o Sistema Financeiro para que o mesmo possa gerar a respectiva cobrança ao aluno.

**R8**- O sistema deve manter informações sobre os alunos e seus históricos escolares

**R9**- O sistema deve permitir aos professores cadastrarem as atividades acadêmicas avaliativas por disciplina que lecionam incluindo uma descrição, a pontuação, e a data de entrega/realização

## Casos de uso

**Visualizar notas**

Classificação: **ALTA**

Justificativa: Processo primário do negócio do cliente

**Matricular em disciplinas**

Classificação: **ALTA**

Justificativa: Persistência de dados, Lida com várias classes de domínio, Processos primários do negócio do cliente, Dependência para outras funcionalidades

**Cancelar matrícula**

Classificação: **MÉDIA**

Justificativa: Cobertura arquitetural com o sistema financeiro, Não é um processo primário do negócio do cliente

**Buscar informações sobre aluno e histórico escolar**

Classificação: **BAIXO**

Justificativa: Baixo impacto na arquitetura

**Buscar informações das disciplinas**

Classificação: **BAIXO**

Justificativa: Baixo impacto na arquitetura

**Buscar informações sobre professor**

Classificação: **ALTA**

Justificativa: Tem integração direta com outro sistema financeiro, Cobertura arquitetural com o sistema de recursos humanos

**Lanças notas**

Classificação: **ALTA**

Justificativa: Persistência de dados, Processos primários do negócio do cliente

**Cadastrar atividade avaliativa**

Classificação: **ALTA**

Justificativa: Persistência de dados, Processos primários do negócio do cliente

**Abrir turma**

Classificação: **ALTA**

Justificativa: Persistência de dados, Lida com várias classes de domínio,  Processos primários do negócio do cliente

**Alocar professor**

Classificação: **MÉDIA**

Justificativa: Processos primários do negócio do cliente
