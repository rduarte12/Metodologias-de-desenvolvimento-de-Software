
## Introdução

Modelos de processo são “roteiros” que orientam times de desenvolvimento desde a concepção até a entrega e manutenção de um sistema. Eles ajudam a controlar, medir e qualificar a produção, adaptando-se a projetos com diferentes realidades e necessidades.

---

## 1. Modelo Cascata (Waterfall)

O **Modelo Cascata** é sequencial, cada etapa só começa após a conclusão da anterior. Muito utilizado quando os requisitos estão bem definidos e raramente mudam.

**Principais etapas:**  
- _Engenharia de Sistemas_  
- _Análise de Requisitos_  
- _Projeto_  
- _Codificação (Implementação)_  
- _Testes_  
- _Manutenção_  

**Fluxograma do Cascata:**

| Engenharia de Sistemas | → | Análise de Requisitos | → | Projeto | → | Codificação | → | Testes | → | Manutenção |
|-----------------------|---|----------------------|---|--------|---|------------|---|--------|---|------------|

**Vantagens:**
- Processo bem controlado, documentação robusta  
- Fácil de gerenciar em projetos com equipes numerosas

**Limitações:**
- Pouca flexibilidade a mudanças  
- Identificação tardia de erros  
- Não indicado quando há grande incerteza nos requisitos

---

## 2. Modelo de Prototipação

Aqui se constrói protótipos rápidos do sistema para que o cliente possa validar os requisitos.

**Etapas:**  
- Obter Requisitos  
- Elaborar Projeto Rápido  
- Construir Protótipo  
- Avaliar Protótipo  
- Refinar Protótipo  
- (Repete enquanto necessário)  
- Construção do Produto Final  

**Fluxo:**

| Obter Requisitos → Elaborar Projeto Rápido → Construir Protótipo → Avaliar Protótipo → Refinar Protótipo → (repete) → Construção do Produto |

**Vantagens:**
- Esclarece necessidades do cliente  
- Permite feedback precoce

**Limitações:**
- Risco do cliente se apegar ao protótipo  
- Comprometimento da qualidade da versão final se o protótipo for aproveitado demais

---

## 3. Modelos Evolutivos

Adotam uma abordagem iterativa, permitindo integração de mudanças contínuas e entregas graduais.

### 3.1 Modelo Incremental

O sistema é desenvolvido e entregue em partes (incrementos), cada um agregando funcionalidades.

**Fluxo:**

| Versão Inicial | → | Versão Intermediária 1 | → | Versão Intermediária 2 | ... | → | Versão Final |

Cada incremento pode passar pelas fases tradicionais (análise, projeto, codificação, teste).

**Vantagens:**
- Valor entregue continuamente ao cliente  
- Adapta-se a mudanças de requisitos ao longo do tempo

**Limitações:**
- Requer bom mapeamento de requisitos para divisão em incrementos  
- Gerenciar integração entre incrementos pode ser desafiador

### 3.2 Modelo Espiral

Criado por Barry Boehm, mescla Cascata e Prototipação, acrescentando a análise de riscos como atividade central.

**Ciclos por fase:**

1. **Planejar (definir objetivos e alternativas)**
2. **Analisar Riscos**
3. **Desenvolver/Validar**
4. **Planejar Próximo Ciclo**

**Fluxo simplificado:**

```
graph TD:
    A([Início]) --> B([Definir Objetivos])
    B --> C([Identificar Avaliar Riscos])
    C --> D([Desenvolver e Validar])
    D --> E([Planejar Próxima Iteração])
    E --> B

```

**Destaques:**
- Flexibilidade e foco contínuo em riscos
- Indicado para projetos longos, complexos e de alto risco
- Exige equipe experiente em identificação e mitigação de riscos

---

## 4. Métodos Formais

Baseiam-se em especificações matemáticas para garantir que o sistema não terá ambiguidades, inconsistências nem imprecisões.

**Usado em:**
- Aeronáutica
- Sistemas de segurança crítica
- Medicina, controle industrial, etc.

**Prós:**
- Altíssimo grau de confiabilidade e precisão

**Contras:**
- Alto custo e complexidade
- Difícil comunicação com stakeholders não técnicos
- Pouco utilizado no mercado convencional

---

## 5. Modelos Ágeis (scrum, XP, Kanban)

Não estavam nos slides, mas são indispensáveis em engenharia de software moderna.

**Características principais:**
- Iterações curtas, entregas frequentes (sprints)
- Reuniões diárias para alinhamento
- Flexibilidade à mudança de requisitos
- Foco na colaboração e comunicação

**Fluxo simplificado:**

| Product Backlog | → | Sprint Planning | → | Sprint | → | Review | → | Retrospective | → | (Novo Ciclo) |

---

## Comparação entre Modelos

| Modelo         | Vantagens                          | Limitações                    | Quando usar                          |
|----------------|------------------------------------|-------------------------------|--------------------------------------|
| Cascata        | Documentação, controle, previsível | Rígido, pouco adaptável       | Requisitos bem definidos             |
| Prototipação   | Esclarece requisitos, iterativo    | Pode comprometer qualidade    | Requisitos incertos                  |
| Incremental    | Entregas contínuas, flexibilidade  | Integração, mapeamento        | Recursos ou requisitos indefinidos   |
| Espiral        | Gestão de riscos, flexível         | Complexo, alta experiência    | Sistemas longos/críticos             |
| Formal         | Precisão, segurança                | Custo, pouca comunicação      | Sistemas críticos/alta confiabilidade|
| Ágeis          | Adaptação, entregas rápidas        | Exige colaboração, disciplina | Mudanças frequentes, projetos dinâmicos |

---

## Conclusão

Não existe modelo universal. A escolha depende de fatores como criticidade, clareza de requisitos, cultura da organização, equipa e recursos. Em muitos casos, modelos são combinados para tirar proveito dos pontos fortes de cada abordagem.

**Leituras recomendadas:**  
- Sommerville, Ian. _Engenharia de Software_  
- Pressman, Roger S. _Engenharia de Software_  
- SWEBOK, IEEE

---

[^1]: Aula04-ModelosProcessoSoftware.pdf

[^2]: QualidadeDeProcesso.md

