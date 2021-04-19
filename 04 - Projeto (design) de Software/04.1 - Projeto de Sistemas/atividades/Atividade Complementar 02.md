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

## Fluxo principal (Matricular em disciplinas)

**Sumário**: O aluno usa o sistema para se matricular em disciplinas.

**Ator primário**: Aluno

**Ator secundário**: Sistema Financeiro

1. O aluno solicita a matrícula em disciplinas
2. O sistema apresenta a lista de disciplinas disponíveis para o semestre corrente para as quais o alunos possui pré-requisitos
3. O aluno seleciona as disciplinas desejadas e solicita a matrícula
4. O sistema aloca o aluno em turmas de ofertas das disciplinas desejadas e informa ao aluno a turma alocada para cada disciplina bem como o professor, os horários e dias da semana e as salas de aula. 
5. O aluno confirma as alocações feitas
6. O sistema realiza a matrícula e envia os dados para o Sistema Financeiro.
7. O caso de uso termina

## Cenário de sucesso do fluxo principal onde o aluno conseguiu se matricular nas disciplinas que solicitou

**Sumário**: O aluno usa o sistema para consultar a grade curricular da disciplina e a bibliografia.

**Ator primário**: Aluno

**Ator secundário**: Sistema de registro acadêmico

1. O aluno solicita detalhes de uma discipĺina que ele esta cadastrado
2. O sistema retorna uma lista de disciplina disponíveis 
3. O aluno seleciona a disciplina que ele deseja verificar informações
4. O sistema retorna uma lista de opções de informações que o usuário pode verificar
5. O aluno seleciona a aba grade curricular e analisa todos os tópicos que serão abordados durante o semestre
6. O aluno seleciona a bibliografia e ve todos os livros que ele pode fazer aquisição para estudar para a prova
7. O aluno encerra a consulta
9. O caso de uso termina


## Cenário onde o aluno solicita mas não consegue realizar a matrícula em todas as disciplinas mas decide entrar em lista de espera.

1. O aluno solicita a matrícula em disciplinas
2. O sistema apresenta a lista de disciplinas disponíveis para o semestre corrente para as quais o alunos possui pré-requisitos
3. O aluno seleciona as disciplinas desejadas e solicita a matrícula
4. O sistema informa que não há mais vagas para a disciplina e pergunta se o usuário gostaria de entrar na fila de espera
5. O usuário aceita entrar na fila de espera
6. O sistema aloca o aluno em turmas de ofertas das disciplinas desejadas e informa ao aluno sua posição na fila. 
7. O aluno confirma as alocações feitas
8. O sistema realiza a matrícula e envia os dados para o Sistema Financeiro.
9. O caso de uso termina