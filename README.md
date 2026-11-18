<p align="center">
  <img src="app/src/main/res/drawable/smile01.png" width="90" alt="Smile triste" />
  &nbsp;&nbsp;
  <img src="app/src/main/res/drawable/smile06.png" width="90" alt="Smile neutro" />
  &nbsp;&nbsp;
  <img src="app/src/main/res/drawable/smile11.png" width="90" alt="Smile feliz" />
</p>

<h1 align="center">Xô Tristeza — Android Nativo com Java</h1>

<p align="center">
  App didático de Android nativo usado nas aulas de <strong>Desenvolvimento Mobile com Android nativo (Java)</strong> que ministro no <strong>Centro Universitário IBMR (Ânima Educação)</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Android%20Studio-3DDC84?style=flat&logo=androidstudio&logoColor=white" alt="Android Studio" />
  <img src="https://img.shields.io/badge/status-conclu%C3%ADdo-success?style=flat" alt="Status: concluído" />
  <img src="https://img.shields.io/badge/IBMR-%C3%82nima%20Educa%C3%A7%C3%A3o-1F3A93?style=flat" alt="IBMR - Ânima Educação" />
</p>

---

## Sobre este repositório

O **Xô Tristeza** foi desenvolvido junto com os alunos nas aulas de **Desenvolvimento Mobile com Android nativo (Java)** que ministro no **Centro Universitário IBMR (Ânima Educação)**.

A proposta é simples e divertida: na tela aparece um smile triste, e cada clique no botão deixa o smile um pouco mais feliz. A cada 10 cliques a imagem muda, passando por 11 expressões, até o smile chegar à felicidade total aos 100 cliques.

A brincadeira prende a atenção da turma e cria um motivo real para escrever código. Os alunos querem ver o smile mudar, testam, alteram as regras e experimentam novas faixas de cliques e novas imagens. Com isso, praticam lógica de programação em Java e os fundamentos do desenvolvimento Android sem perceber o esforço.

Esta é a versão do app desenvolvida com as turmas do IBMR, Ânima Educação.

> ✅ **Projeto concluído:** o app está completo e serve como gabarito para revisão e prática dos alunos.

## Como o app funciona

| Ação do usuário | O que acontece |
|---|---|
| Clica no botão **"Clique aqui e seja feliz!"** | O contador soma 1 e o número aparece na tela |
| Chega a 10, 20, 30 … 100 cliques | O smile troca para uma expressão mais feliz |
| Clica no texto **"Zerar Contador"** | O contador volta a 0 e o smile volta a ficar triste |

## O que se aprende com este app

- **Estrutura de um projeto Android:** `Activity`, ciclo de vida com `onCreate()`, layout em XML e a classe `R`
- **Ligação entre XML e Java:** recuperar componentes com `findViewById()`
- **Dois jeitos de tratar cliques:**
  - no **Button**, com `setOnClickListener()` e uma classe anônima `View.OnClickListener`
  - em uma **View que não é Button** (um `TextView`), com o atributo `android:onClick` no XML apontando para um método público da Activity
- **Lógica de programação em Java:** atributo contador, incremento (`contador++`) e a estrutura de decisão `switch/case`
- **Atualização da interface em tempo real:** `setText()` com conversão de tipo via `String.valueOf()`
- **Imagens via código:** troca da imagem de um `ImageView` com `setImageResource()` usando recursos da pasta `drawable`
- **Layout com ConstraintLayout:** posicionamento de `ImageView`, `TextView` e `Button`

## Tecnologias

| Categoria | Ferramentas |
|---|---|
| Plataforma | Android nativo |
| Linguagem | Java |
| IDE | Android Studio |
| Layout | XML com ConstraintLayout |
| Configuração | compileSdk 34 · minSdk 28 (Android 9) |

## Estrutura do projeto

```
app/src/main/
├── java/.../MainActivity.java     # Lógica do contador, do switch/case e da troca de imagens
├── res/layout/activity_main.xml   # Tela: ImageView, contador, botão e texto "Zerar"
└── res/drawable/smile01 … smile11 # As 11 expressões do smile, da tristeza à felicidade
```

Pacote: `br.com.fabriciocurvello.appxotristezaanima`

## Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/fabcurvello/AppXoTristezaAnima.git
   ```
2. Abra a pasta do projeto no **Android Studio** e aguarde a sincronização do Gradle.
3. Execute em um emulador ou em um celular Android com a depuração USB ativada.

## Desafios para praticar

- Mudar as faixas de cliques em que o smile troca de expressão
- Substituir o `switch/case` por uma estrutura `if/else` ou por um array de imagens
- Mostrar um `Toast` de parabéns quando o smile ficar totalmente feliz
- Manter o valor do contador ao girar a tela

## Sobre o professor

**Fabricio Curvello** é desenvolvedor e professor de desenvolvimento de software. Leciona no SENAI-RJ desde 1997, em cursos de programação, banco de dados, web e desenvolvimento fullstack, e no Centro Universitário IBMR desde 2018, nos cursos de Análise e Desenvolvimento de Sistemas, Ciência da Computação e Gestão de TI.

No desenvolvimento mobile, usa apps curtos, visuais e divertidos como este para ensinar Android nativo com Java. A ideia é que cada conceito apareça funcionando na tela do celular do aluno, o que mantém a turma motivada e torna a prática de código mais eficiente.

- LinkedIn: [linkedin.com/in/fabriciocurvello](https://www.linkedin.com/in/fabriciocurvello)
- YouTube: [@fabriciocurvello](https://www.youtube.com/@fabriciocurvello)
- GitHub: [github.com/fabcurvello](https://github.com/fabcurvello)
- Currículo Lattes: [lattes.cnpq.br/2406072276749635](http://lattes.cnpq.br/2406072276749635)

---

<p align="center">
  Material de apoio às aulas de Desenvolvimento Mobile do Centro Universitário IBMR (Ânima Educação).
</p>
