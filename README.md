# SIRIUSAeB
APLICAÇÃO DE GESTÃO DE SAÚDE SIRIUS A&amp;B
Sirius A&B — Gestão Inteligente de Saúde, 
Cuidado e Segurança Ativa 
O Sirius A&B é uma aplicação web moderna (Single-Page Application) desenvolvida como 
parte da Prática Profissional Supervisionada do Instituto Benjamin Constant (IBC), no 
âmbito do Curso Técnico de Nível Médio em Inteligência Artificial. O sistema foi projetado 
para oferecer acompanhamento contínuo de saúde, gestão da rotina de medicamentos, 
análise preditiva de sinais de bem-estar e segurança ativa. 
Objetivo e Públicos-Alvo (Três Ambientes Integrados) 
A proposta central do Sirius A&B é atender três cenários fundamentais de cuidado em 
ambientes separados e personalizados por conta e perfil de acesso: 
1.  Monitoramento de Idosos (Perfil Cuidador / Familiar): Acompanhamento rigoroso 
de medicações, controle de pressão arterial/glicemia, agenda de consultas e 
prevenção de emergências. 
2.  Suporte para Mães Atípicas (Perfil Cuidador): Diário de cuidados com transcrição 
por voz para registrar comportamentos, sintomas ou rotinas terapêuticas de forma 
ágil, gerando resumos automáticos para médicos e especialistas. 
3.  Pessoas que Moram Sós (Perfil Cliente Independente): Autogestão de saúde 
aliada ao sistema de Segurança Ativa (monitoramento periódico de bem-estar e 
acionamento automático de contatos de emergência caso não haja resposta). 
4.  Gestão do Sistema (Perfil ADM): Painel administrativo para controle, exportação e 
limpeza segura de registros. 
Funcionalidades do Projeto 
Recursos Inteligentes (Integrados ao Projeto Cuidador de Pessoa) 
● Leitura Inteligente de Receitas e Caixas de Bulas (OCR Real): Utiliza a câmera ou 
upload de fotos com Tesseract.js para ler o texto impresso na embalagem do remédio 
ou receita, preenchendo automaticamente o nome do medicamento, a dosagem (mg, 
ml, mcg, gotas, comprimidos) e o horário sugerido. 
● Transcrição de Voz para o Diário de Cuidados: Permite registrar anotações diárias 
utilizando ditado por voz, facilitando a rotina de cuidadores e mães atípicas. 
3
● Resumos Automáticos: Geração instantânea de relatórios consolidados por período 
(Hoje, Últimos  dias, Última semana ou Último mês) prontos para copiar e enviar ao 
médico. 
● Análise Preditiva e de Padrões de Saúde: Avaliação automática dos dados 
registrados com geração de insights de estabilidade ou alertas de risco (como picos 
hipertensivos). 
● Detecção de Interação Medicamentosa: Análise preventiva da lista de 
medicamentos ativos na rotina do paciente. 
● Assistente "Chatbot" no Próprio Site: Assistente virtual Sirius integrado no canto 
inferior da tela para suporte rápido ao usuário. 
Base Estrutural Implementada 
● Gerenciamento da Rotina de Medicamentos: Controle diário de doses, horários, 
previsão de continuidade e marcação de medicamentos já tomados. 
● Registro de Sinais de Bem-Estar: Monitoramento de Pressão Arterial 
(Sistólica/Diastólica), Frequência Cardíaca (bpm), Glicemia (mg/dL) e escala visual de 
Humor/Bem-estar, acompanhados de gráficos evolutivos interativos (Chart.js). 
● Geração de Alertas e Botão de Pânico (Segurança Ativa): 
● Verificação periódica programável e acionamento imediato de teste/pânico. 
● Emissão de alarme sonoro real (via Web Audio API) nos horários agendados. 
● Contagem regressiva em tempo real: caso o usuário não confirme clicando em 
"ESTOU BEM" dentro do tempo limite, o protocolo de socorro aciona os 
contatos de emergência cadastrados e o SAMU ( ). 
192
● Autenticação com Senha Fixa e Isolamento por E-mail: 
● Sistema completo de Cadastro, Login validado e Recuperação de Senha 
("Esqueci minha senha"). 
● Banco de dados local (localStorage) particionado por e-mail: cada conta 
possui seus próprios registros, fotos e perfis 100% separados. 
Tecnologias Utilizadas 
● HTML5 & CSS3: Estrutura semântica e responsiva. 
● Tailwind CSS (via CDN): Interface moderna com Glassmorphism e adaptação total 
para celulares e desktops. 
● JavaScript (ES6+): Gerenciamento de estado multiusuário, banco de dados local 
isolado por e-mail e agendadores em tempo real. 
● Chart.js: Gráficos dinâmicos de evolução dos sinais vitais. 
● Tesseract.js (v5): Motor de Reconhecimento Óptico de Caracteres (OCR) executando 
diretamente no navegador. 
● Web Audio API & Web Notifications API: Sintetizador de alarme sonoro de 
emergência e notificações Push. 
● Font Awesome 6: Ícones médicos e visuais. 
Como Executar o Projeto 
Como o Sirius A&B foi arquitetado em um arquivo único autocontido (index.html), não é 
necessário instalar dependências complexas para rodá-lo: 
1: Hospedagem na Nuvem (Netlify / Vercel / GitHub Pages) 
1. Acesse o Netlify. 
2. Arraste o arquivo index.html diretamente para a área de Upload (ou conecte este 
repositório do GitHub). 
3. Seu aplicativo estará online imediatamente com certificado de segurança HTTPS! 
Estrutura de Arquivos do Repositório 
None 
�
�
SIRIUSAB 
┣ 
�
�
 index.html                        
Lógica JS) 
┣ 
�
�
 README.md                         
projeto 
# Aplicação completa (Interface, Estilos e 
┣ 
�
�
 relatorio_alteracoes_sirius_ab.md # Relatório técnico detalhado de 
desenvolvimento 
┣ 
�
�
 app_transformation_guide.md       
Android/iOS 
┣ 
�
�
 pwa_builder_guide.md              
PWABuilder 
┗ 
�
�
 github_step_by_step_guide.md      
# Documentação principal e concepção do 
# Guia para converter em aplicativo 
# Passo a passo de publicação via 
# Guia de versionamento e deploy no GitHub 
Autores e Equipe de Desenvolvimento 
● Ana Paula Quadros Desidério 
● Beatriz de Sousa Falcão 
● Ítalo Augusto Costa dos Santos 
Dados Acadêmicos 
● Instituição: Instituto Benjamin Constant – IBC 
● Curso: Curso Técnico de Nível Médio em Inteligência Artificial 
● Atividade: Prática Profissional Supervisionada
