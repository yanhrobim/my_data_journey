# 📒 Diário de Estudos - (Excel)

## 📌 Objetivos dos Estudos

Aprender fundamentos e conceitos da ferramenta **Excel**, incluindo fórmulas, funções de busca, **tabelas dinâmicas** e gráficos, através do curso **Excel Básico Office 365** da **Hashtag Treinamentos**.
Com o objetivo de aprender sobre a ferramenta, consolidar conhecimento e aplicá-lo em um projeto de análise de dados (RH), complementando o que já foi estudado em **Power BI**.

---

## 📝 Registro Por Aula

### | 📚 Aula 1

#### **Dia 1 (05/11/26)**

**🖋️ Tópicos da Aula:**
- Conceitos Introdutórios
- Atalhos
- Preenchimento Relâmpago

**🧠 Aprendizados da aula:**
- **Apresentação da interface da ferramenta e conceitos introdutórios:**
    - O que é uma pasta de trabalho.
    - O que é uma planilha dentro de uma pasta de trabalho.
    - O que é uma coluna, linha, e célula (encontro de linhas com colunas).
    - Guias e suas ferramentas.
- Importação de arquivo Text/CSV dentro do Excel.
- Descoberta de **atalhos** dentro da ferramenta para se locomover melhor entre os dados e ganhar tempo.
    - Exemplos Básicos:
        - CTRL + Page Up e CTRL + Page Down para se locomover sem utilizar o mouse entre planilhas.
        - CTRL + ⬆️, CTRL + ⬇️,  CTRL + ➡️, CTRL + ⬅️ para se locomover mais rápido entre os dados da planilha.
- Com o preenchimento relâmpago conseguimos fazer com que o Excel replique uma lógica que aplicamos entre os dados. 
- **Preenchimento Relâmpago (Flash Fill):**
  - **O que é:** um recurso em que eu mostro ao Excel *um exemplo* do resultado que quero, e ele descobre o padrão e preenche o resto da coluna sozinho, sem fórmula.
  - **Atalho:** `CTRL + E` (aplica o preenchimento relâmpago na hora, depois de eu digitar o exemplo na primeira célula).
    - ⚠️ **Aviso:** esse atalho pode variar conforme a versão do Excel ou o sistema operacional (no Mac, por exemplo, costuma ser `CMD + E`).
  - **Como usar:** digito o resultado esperado na primeira célula ao lado dos dados, começo a digitar o segundo, e o Excel sugere o restante. Se ele não sugerir sozinho, uso o atalho.
  - **Exemplo:** coluna com "João Silva". Na célula ao lado escrevo "João", e o Excel preenche só o primeiro nome de todas as outras linhas.
  - **Para que serve:** separar, juntar ou reformatar textos (nomes, e-mails, telefones) de forma rápida.
  - **Cuidado:** ele *adivinha* o padrão, então pode errar se os dados forem irregulares. Sempre conferir o resultado.

---

### | 📚 Aula 2

#### **Dia 2 (10/11/26)**

**🖋️ Tópicos da Aula:**
- Formatação
- Formatação Condicional

**🧠 Aprendizados da aula:**
- **Formatação:** Formatação é a forma que você mostra as informações que estão no Excel.
	- **Formatação de Valores:** Mudar como o valor da célula será exibido, como números, texto, datas. (Não muda o valor real, e sim como é apresentado)
		- **Exemplo:** Formatar um valor numérico para um valor em moeda.
      - ![formatação_valores](2.%20Formatação%20e%20Formatação%20Condicional/Images/exemplo_formatação_valores.png)
	- **Formatação Visual:** Mudar a aparência da apresentação sem afetar os valores, como cores, fontes, bordas.
		- **Exemplo:** Adicionar Bordas e Cores.
      - ![formatação_visual](2.%20Formatação%20e%20Formatação%20Condicional/Images/exemplo_formatação_visual.png)
	- **Atalho:** `CTRL + 1` para abrir um menu avançado sobre formatação. (Incluí tanto a formatação de valores quanto a formatação visual)
- **Formatação Condicional:** Aplica formatações visuais em células através de uma regra.
	- **Exemplo:** Se na coluna `Nivel_Satisfacao_Trabalho` a nota for 1, preencha com emoji vermelho, se for de 2 emoji amarelo, e se for 3 e 4 com emoji verde. (Com base em: Ruim, Médio, Bom)
  - ![formatação_condicional](2.%20Formatação%20e%20Formatação%20Condicional/Images/exemplo_formatação_condicional.png)
  - **OBS:** Caso o valor da célula seja modificado a aparência também é automaticamente modificada.


---

### | 📚 Aula 3

#### **Dia 3 (11/11/26)**

**🖋️ Tópicos da Aula:**
- Validação de Dados
- Tabelas (Classificar e Filtrar)

**🧠 Aprendizados da aula:**

- **Validação de Dados no Excel:** Impedir com regras que valores indevidos não entrem na planilha.
	- Existe variedades de regras de validação de dados dentro do Excel. Estas foram as que utilizei e irei cita-las aqui como exemplo:
		- **É maior que (Neste caso é 0):**
		- ![regra_maior_que](./3.%20Validação%20de%20Dados%20e%20Tabelas/Images/regra_numero_maior_que.png)
		- Com o objetivo de somente ter valores numéricos em ID.
		- **Lista de Valores Aceitos:**
		- ![regra_valores_aceitos](./3.%20Validação%20de%20Dados%20e%20Tabelas/Images/regra_valores_aceitos.png)
		- Com o objetivo de na coluna não conter Estados Civis incorretos. (No momento de análises, se tiver, deixa os dados não confiáveis/sujos.)
		- **Números Entre Valor X até Valor Y:**
		- ![regra_numeros_entre](./3.%20Validação%20de%20Dados%20e%20Tabelas/Images/regra_numeros_entre.png)
		- Com o objetivo de fazer com que na coluna `Idade` esteja somente pessoas de 18 a 60 anos.
	- ***Para a utilização da ferramenta de validação de dados no Excel, é preciso entrar na Guia `Dados`.***
- A principal importância de utilizar **Tabelas** no Excel é que ela facilita a replicação de regras de validação, fórmulas, funções em novas linhas de forma automática.
	- Sem **Tabela**, os dados ficam soltos na planilha. Quando adiciono uma nova linha, ela nasce “individual”: as outras colunas existem, mas vazias, e a nova linha não herda as regras de validação, as fórmulas nem as funções das linhas de cima.
	- Com **Tabela**, a nova linha já nasce seguindo tudo isso, sem eu precisar copiar ou arrastar nada.


---

### | 📚 Aula 4

#### **Dia 4 (12/11/26)**

**🖋️ Tópicos da Aula:**
- Tabela Dinâmica
- Segmentação de Dados

**🧠 Aprendizados da aula:**
- **Tabelas Dinâmicas:** Permite fazer e criar análises de forma claras e objetivas. Em muitos casos utilizamos **Fórmulas** e **Funções** para criar e fazer análises mais complexas, porém, se você quer uma análise mais rápida e pontual, uma melhor escolha é a **Tabela Dinâmica**.
- ![tabela_dinamica](./4.%20Tabelas%20Dinâmicas%20e%20Segmentação%20de%20Dados/Images/tabela_dinamica.png)
-  **Como a Tabela Dinâmica funciona por dentro:**
	- **Criar:** Inserir → Tabela Dinâmica, escolhendo a origem. Depois é arrastar os campos nas 4 áreas: Filtros, Colunas, Linhas e Valores.
	- **Cache:** quando a Dinâmica nasce, o Excel tira uma cópia dos dados. É por isso que ela não vê linha nova sozinha, e por isso o Atualizar é manual.
	- **Origem:** escolher a **Tabela** (`Ctrl + T`), nunca o intervalo fixo (`A1:D500`). Intervalo fixo ignora a linha nova em silêncio: o resumo fica errado sem avisar.
	- **Célula calculada:** não dá para digitar dentro dela. Ali não tem dado, tem conta.
	- **Datas:** botão direito sobre a data → Agrupar, para ver por mês, trimestre ou ano.
- **Qual a diferença de Tabela x Tabela Dinâmica?**
	- A diferença é que a **Tabela** armazena dados, e a **Tabela Dinâmica** entrega dados calculados, entrega respostas para perguntas de negócio, semelhante a uma Query de KPI em SQL.
		- Nos nossos dados de RH, por exemplo ver qual a nota que mais aparece na `Nivel_Satisfacao_Trabalho` por `Funcao` (Cargo). (Ajudaria entender por que certos cargos estão mais descontentes que outros.)
	- OBS: Quando a Tabela que alimenta a Tabela Dinâmica é atualizada por dados, o filtro prevalece SE estes novos dados seguem e contém dados que alimentam o filtro.
		- **Por exemplo:** Se você antes apontava para Cargos como "Engenheiro de Dados", "Analista de Dados" e "Cientista de Dados" e os dados sofreram uma atualização agora sendo "DE", "DA" e "DS", a Tabela Dinâmica não entrega nada.
- **Segmentação de Dados** é o nome em português do **Slicer**: botões de filtro que ficam visíveis na tela, em vez de escondidos na setinha da coluna.
- Inserir → Segmentação de Dados com a Dinâmica selecionada. Uma caixinha agora visível na tela, que você pode clicar para filtrar por aquilo que escolheu. (Ex: Por `Funcao`)

---

### | 📚 Aula 5

#### **Dia 7 (17/11/26)**

**🖋️ Tópicos da Aula:**
- Gráficos

**🧠 Aprendizados da aula:**
- O real objetivo de utilizar/trabalhar com *Gráficos* é demonstrar dados de forma visual, como no Power BI, entre outras ferramentas de visualização de dados.
- **Existe Duas Formas Para Criar Gráficos Dentro do Excel:**
	- **1. Forma Mais Simples:** Nesta forma mais simples, você apenas clicando o Excel cria um gráfico para você. Para isso você precisa selecionar a sua tabela inteira que contém os dados desejados, na *Guia*: Inserir → Gráficos.
		- ***Está forma é a mais simples e rápida, porém nem sempre ela pode funcionar.*** No meu exemplo, nos meus dados dos vendedores somente tenho o ID, quando tentei por esse caminho criar um gráfico que representasse de forma visual aqueles que venderam mais quantidades, o Excel não soube diferenciar os IDs do valor de quantidade vendida e assim com este método não soube popular o eixo X com os valores de IDs.
	- **2. Forma Mais Complexa:** Diferentemente da primeira forma, aqui você primeiro insere o gráfico que você deseja (Através de Inserir → Gráficos) sem ter que selecionar toda a sua tabela e já popular o gráfico com dados. Com o gráfico em branco, você pode clicar com o botão esquerdo e encontrar a opção: *"Selecionar Dados"*, ou clicar com o botão direito no gráfico e uma nova *Guia* (Localizada sendo a penúltima, antes de Formatar) irá ser criada chamada Design do Gráfico, onde lá se encontra *"Selecionar Dados"*. Após clicar na ferramenta, você precisa adicionar os dados no botão *"Adicionar"*, no lado esquerdo, com isso você precisa criar o nome de uma série e os dados que ela irá ter (Por exemplo, se seus dados são de Vendas, coloque o nome da série "Vendas" e clique na coluna ou tabela que contém os dados). Após isso, você irá popular o eixo Y com os valores selecionados, e para modificar o eixo X você precisa clicar em "Editar" na caixinha do lado direito e selecionar os dados que serão o eixo X (Por exemplo, se no eixo X você quer o nome das Regiões você referencia estes dados).
- **Gráfico Que Eu Criei para Praticar:**
	- ![grafico_aula5](./5.%20Gráficos%20No%20Excel/images/grafico_pratica.png)


---

### | 📚 Aula 6

#### **Dia 8 (24/11/26)**

**🖋️ Tópicos da Aula:**
- Funções Básicas (Operadores, SOMA, MÉDIA, MULT, MAIOR/MENOR, CONT.NÚM/CONT.VALORES)

**🧠 Aprendizados da aula:**
- Para acessar formúlas no Excel é preciso colocar o caracter: **"="**.
- **Prática de Algumas Funções Básicas e Resultados Com Os Dados de Logística (Sobre Vendedores):**
	- **ÚNICO():**
		- ![unico_funcao](./6.%20Funções%20Básicas/images/funcao_unico_resultado.png)
		- Dentre os dados de logística, individualizar cada ID de Vendedor, com o objetivo de obter os vendedores de forma individual.
	- **CONT.VALORES():** ou **CONT.VALORES(ÚNICO()):**
		-  ![cont_valores_funcao](./6.%20Funções%20Básicas/images/funcao_cont_valores_resultado.png)
		- Contagem de valores (vendedores).
	- **MÉDIA():**
		- ![media_funcao](./6.%20Funções%20Básicas/images/funcao_media_funcao.png)
		- Obter uma média dentre um conjunto de valores númericos passados.
	- **SOMA():**
		- ![soma_funcaop](./6.%20Funções%20Básicas/images/funcao_soma_resultado.png)
		- Fazer uma conta de adição dentre os valores númericos passados.

---

### | 📚 Aula 7

#### **Dia X (DD/MM/AA)**

**🖋️ Tópicos da Aula:**
- Função SE
- Função PROCV

**🧠 Aprendizados da aula:**

---

### | 📚 Aula 8

#### **Dia X (DD/MM/AA)**

**🖋️ Tópicos da Aula:**
- Função CONT.SES
- Função SOMASES

**🧠 Aprendizados da aula:**

---