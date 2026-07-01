# Desafio Criativo - Extraindo Insights do Feedback de Clientes Bancários

Este repositório contém a resolução do Desafio Criativo proposto no Bootcamp da [DIO](https://www.dio.me) em parceria com o **Bradesco**. O objetivo principal é estruturar prompts eficientes para Inteligência Artificial Generativa, focando em extrair percepções valiosas de feedbacks reais de clientes, abordando o cenário crítico de segurança e prevenção a golpes no ecossistema do Pix.

---

## Tema Escolhido: Segurança no Pix e Prevenção a Golpes

### Passo 1: Defina a intenção

**Quero que a IA analise** relatos de contestação de fraudes, reclamações sobre golpes envolvendo o Pix e comentários sobre o acionamento do suporte de emergência nas redes sociais e canais de ouvidoria **para identificar** falhas graves de comunicação, pontos de lentidão no bloqueio cautelar da conta e o nível de entendimento dos usuários sobre o Mecanismo Especial de Devolução (MED).

**O resultado será usado por** analistas da equipe de Prevenção a Fraudes, gestores de Experiência do Cliente e a gerência de Canais Digitais **para apoiar** a reestruturação dos fluxos de atendimento pós-golpe e o refinamento das travas de segurança preventiva no aplicativo.

**A entrega deve conter** um diagnóstico analítico da percepção de segurança do cliente, um resumo executivo sintetizando o principal sentimento das vítimas, uma tabela detalhada mapeando as maiores frustrações por tipo de incidente com exemplos reais, e um plano com 3 recomendações prioritárias de curto prazo.

**O resultado será considerado bom se** conseguir traduzir a dor e o desamparo do cliente em gargalos processuais claros que o banco possa corrigir, diferenciando problemas de usabilidade do aplicativo de falhas no atendimento humano ou de limitações da própria regra do Banco Central.

---

### Passo 2: Adicione contexto e restrições

**Contexto:** Estou trabalhando com feedbacks de clientes bancários relacionados a incidentes reais de segurança digital, focando especificamente no fluxo que ocorre após o cliente sofrer um golpe (como engenharia social, Pix sob coação ou acesso não autorizado) e precisar da ajuda urgente do banco. O foco é entender se o banco é visto como um parceiro ágil ou como uma barreira burocrática em momentos de estresse financeiro extremo.

**Dados disponíveis:** A base de dados fornecida contém a data e hora exata do registro, o canal digital de origem (como Reclame Aqui ou redes sociais), a descrição textual do relato detalhado feita pelo cliente, a faixa estimada do prejuízo financeiro sofrido e o status final do atendimento na ouvidoria (concluído, em análise ou sem resposta).

**Critérios de análise:** A IA deve classificar os feedbacks correlacionando o tipo de golpe sofrido com o sentimento predominante da vítima (como urgência, raiva ou desamparo), identificar se a comunicação das regras de reembolso foi transparente e mapear em qual etapa do suporte (espera no chat, transferência de setor ou envio de boletim de ocorrência) o cliente encontrou maior dificuldade.

**Cuidados e restrições:**
* Use exclusivamente os dados textuais fornecidos, sem extrapolar para estatísticas de mercado que não estejam na base.
* Não invente culpados, causas técnicas ocultas ou conclusões sem evidências diretas nos relatos.
* Não exponha, sob nenhuma hipótese, dados pessoais, nomes, agências, CPFs ou chaves Pix presentes nos textos originais.
* Indique claramente as limitações da análise caso faltem informações cruciais sobre o desfecho do caso.
* Utilize uma linguagem analítica, séria, empática com a dor do cliente, mas totalmente voltada para ações corporativas e tomada de decisão estratégica.

---

### Passo 3: Prompt Final (Pronto para a IA)

```text
Atue como especialista em segurança da informação e analista de experiência do cliente no setor bancário.

Sua tarefa é analisar manifestações e reclamações de clientes vítimas de fraudes e golpes envolvendo transações via Pix sobre os canais digitais e o atendimento de emergência para identificar os principais gargalos no suporte emergencial, a clareza nas orientações fornecidas e oportunidades de melhoria na segurança preventiva.

Contexto: A análise será utilizada pelas equipes de Prevenção a Fraudes e de Experiência do Cliente. O objetivo principal é alimentar esses times com percepções valiosas para desenhar jornadas de atendimento mais ágeis, humanas e eficientes, minimizando o impacto emocional e financeiro sofrido pelo cliente durante incidentes de segurança.

Dados disponíveis: Serão fornecidos relatos textuais que contêm a data do registro, o canal de origem do comentário, a descrição detalhada do ocorrido, a faixa de valor da perda financeira e a situação do atendimento na ouvidoria.

Instruções de análise:
1. Classifique os feedbacks agrupando-os pelo tipo de incidente (Ex: golpe do falso funcionário, Pix sob coação, invasão de conta) e pelo sentimento da vítima.
2. Identifique as principais travas e atritos enfrentados no fluxo de suporte (Ex: lentidão para bloquear a conta, falta de entendimento sobre o Mecanismo Especial de Devolução).
3. Aponte evidências qualitativas indiscutíveis nos dados, selecionando pequenas frases ou citações marcantes extraídas diretamente dos comentários.
4. Sugira ações de comunicação educativa bem diretas e melhorias práticas nos alertas preventivos que aparecem dentro do aplicativo do banco.

Formato da resposta: Entregue um resumo executivo analítico de até 6 linhas focado na percepção de segurança da marca; uma tabela estruturada contendo (Tipo de Incidente | Principal Frustração Relatada | Citação da Evidência | Ação Recomendada); e, por fim, uma lista contendo 3 propostas textuais de alertas de segurança preventivos para serem implementados no aplicativo.

Restrições:
* Apoie-se unicamente nas informações enviadas, sem criar dados fictícios ou conclusões sem base.
* Não invente culpados ou métricas de eficácia que os dados não sustentem.
* Mantenha sigilo absoluto e omita/mascare qualquer dado pessoal ou sensível presente nos relatos.
* Se a base não permitir rastrear o desfecho de um problema, reporte essa limitação explicitamente.
* Adote um tom sério, corporativo, analítico e focado em soluções ágeis.
