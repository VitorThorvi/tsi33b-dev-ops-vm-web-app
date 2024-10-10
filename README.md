# tsi33b-dev-ops-vm-web-app

## Assignment 1 - Virtualized Web Application

Assignment roadmap and development process is described on [roadmap.md](roadmap.md) on root dir of this repo.

This project is developed under the context of UTFPR TSI323B course. This application is intended for graduate study program purposes. 

### Objective:
The student is expected to **demonstrate its ability to work with web application virtualization.**

---

#### Task Description:
Customize and virtualize a CRUD web application to meet the needs of a fictional company. Then, record a video explaining the virtualization process and show the application running on VM's.

## Steps - Requirements (REQ) and evaluation Criteria (CRIT)

Below is a step-by-step guide detailing what to do at each stage. 

### Evaluation Criteria

CRIT01 - Atender ao enunciado e aos requisitos (REQ) apresentados;

CRIT02 - Originalidade. Se foi você que fez e se funcionou, muito bem! Não se preocupe em falar muito bem e/ou se apresentar muito bem, apesar que é bom, pois muitas empresas consideram uma boa apresentação em entrevistas de emprego;

CRIT03 - Competência. Mostre a sua competência, se você realmente entendeu o que fez e se é capaz de fazer esse tipo de trabalho;

CRIT04 - Transparência. Seja verdadeiro(a), ninguém sabe tudo, talvez alguma implementação que gostaria de fazer, mas não conseguiu ou não deu certo;

CRIT05 - Diferencial. Algo diferencial mostrará que você conseguiu fazer além do básico, trouxe algo de novo ou diferente que provavelmente os seus colegas não fizeram.

Pontuação: CRIT01 consoante com os critérios CRIT02, CRIT03 e CRIT04 valem 2 (dois) pontos. CRIT05 vale 1 (um) ponto. Totalizando 3 (três) pontos.

---

### Requirements

#### 1 - Personalização de uma aplicação web CRUD.

Na Internet você encontrará diversas aplicações web CRUD de exemplo, poderá utilizar qualquer uma desde que você respeite os termos e direitos autorais de quem a disponibilizou, busque salvar a sua aplicação, ou seu projeto, de maneira privada.

Personalize a sua aplicação web:

REQ01 - Escolha um nome fictício para a sua empresa, seja criativo para evitar duplicidade com trabalho dos colegas;
REQ02 - Crie um logotipo para sua empresa. Este logotipo deverá aparecer em todas as páginas da sua aplicação;
REQ03 - Escolha um domínio (DNS) para a sua empresa, ex.: empresatal.com.br, este deverá ser usado para URL da sua aplicação;
REQ04 - A aplicação deverá ser somente CRUD, nem um módulo a mais;
REQ05 - A aplicação deverá gravar apenas em uma tabela com no mínimo 3 e no máximo 10 campos (campo = colunas da tabela);
REQ06 - Durante as aulas trabalharemos com aplicações em PHP, mas será permitido utilizar outras linguagens desde que o seu frontend seja HTML/CSS para navegadores Web.
REQ07 - Sem frameworks. Se for o caso, consultar professor antes.
REQ08 - Durante as aulas trabalharemos com bancos de dados MySQL/MariaDB, mas será permitido utilizar outros, desde que seja acessível pela rede - ou seja, não arquivos de texto e nem SQLite.

#### 2 - Virtualize a sua aplicação web CRUD.

Na Internet você encontrará várias formas de disponibilizar uma aplicação web em máquinas virtuais, busque o melhor para a sua aplicação, pense em organização, performance, simplicidade.

REQ09 - Disponibilize a sua aplicação web em máquina virtual acessível por porta 80, opcionalmente porta 443 se preferir HTTPS;
REQ10 - Disponibilize o banco de dados em máquina virtual separada;
REQ11 - Configure acesso via URL com FQDN, exemplo http://www.site.com, utilize o arquivo hosts na estação cliente. Opcionalmente, se achar melhor, instale e configure um servidor de DNS.
REQ12 - Crie um pequeno tutorial com os passos necessários para rodar a sua aplicação.

#### 3 - Implemente um diferencial:

Implemente algo diferente/melhor, por exemplo, utilizar outras distribuições, outro virtualizador, outra linguagem, outro banco de dados. Subir um serviço adicional como tratamento de logs, monitoramento. Implementar algum serviço de segurança adicional. Etc. Procure não descaracterizar o trabalho quebrando alguns dos requisitos aqui listados, se for o caso contate o professor antecipadamente.

#### 4 - Prepare o ambiente de demonstração:

Crie um cenário, desenhe a topologia (ex.: em Draw.IO), prepare um ambiente para gravar seu vídeo de demonstração.

REQ13 - Prepare a topologia, sugestões:
Topologia mínima:
- 1 estação cliente (navegador)
- 1 servidor web
- 1 servidor db
  Topologia ideal:
- 1 estação cliente
- 1 servidor para DNS e CA (opcional)
- 1 servidor web
- 1 servidor db
  Topologia completa: uma máquina virtual para cada serviço se houver recursos computacionais suficientes.

REQ14 - Prepare o cenário, pense no DevOps preparando e subindo a aplicação, pense no internauta/cliente utilizando a aplicação, pense no público que assiste ao seu vídeo;
REQ15 - Procure deixar sua gravação de tela nítida, se necessário aumente as fontes de editores/navegadores e terminais.

Sugestão: grave um vídeo (sem áudio ainda) deste cenário sendo executado, depois faça cortes e edição para atender ao próximo passo.

#### 5 - Grave o seu Vídeo Explicativo.

Se o passo anterior resultou em um vídeo editado, prossiga neste passo gravando você explicando o seu trabalho. Se achar melhor, pode fazer um vídeo apenas atendendo à este passo e ao anterior.

REQ16 - Grave seu rosto quando estiver explicando para que possamos reconhecê-lo;
REQ17 - Grave sua voz nitidamente;
REQ18 - Seu vídeo deve ter no máximo 12 minutos (não extrapolar). Ideal se for entre 7 e 10 minutos.

Sugestão: você pode utilizar o Google Meet como aluno(a) da UTFPR (seulogin@alunos.utfpr.edu.br) e gravar e salvar este vídeo no Google Drive.

#### 6 - Poste o seu Vídeo.

REQ19 - Pode ser um link do Youtube (não listado) ou link do vídeo armazenado no Google Drive, coloque permissão de acesso para hermanopereira@professores.utfpr.edu.br;
REQ20 - Tome atenção para não enviar link quebrado, link encurtado, link sem permissão de acesso, link de vídeo incompleto e/ou corrompido, link de pasta do Drive, pois o trabalho será simplesmente zerado. Por isso verifiquem e testem antes.

Sugestão: abra e mostre partes importantes do código, como configurações, mostre o tutorial, explique o seu cenário com figuras, localize-se em terminais (estou no servidor, estou na estação), mostre os comandos rodando, mostre sua aplicação funcionando.