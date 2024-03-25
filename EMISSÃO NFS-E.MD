# EMISSÃO DE NOTAS FISCAIS DE SERVIÇO -

---

## Passo 1 - Verificar informações no E-mail

1. Abrir o e-mail (monitoramento.cbapocos@stplog.com.br).
2. Verificar caixa de entrada o e-mail recebido parecido com **_(NFES_21-02-2024_3ª Rodada_STP_Fazenda_da_Inveja_2169)_**, neste e-mail contém todas as informações necessárias para à emissão dos NF-e
3. Manter o e-mail recebido aberto para cópia das informações.

### Exemplo da planilha que chega no e-mail

| MINA  | DMT   | TAG | PLACA   | NF     | Nº FOLHA REG | TONS | PREÇO  | PREÇO c/ ICMS |
| ----- | ----- | --- | ------- | ------ | ------------ | ---- | ------ | ------------- |
| 69-01 | 18A19 | 1   | SCO2D27 | 266950 | 1038048968   | 15   | 321,00 | 337,95        |
| 69-01 | 18A19 | 1   | SCO2D27 | 266950 | 1038048968   | 15   | 321,00 | 337,95        |
| 69-01 | 18A19 | 1   | SCO2D27 | 266950 | 1038048968   | 15   | 321,00 | 337,95        |
| 69-01 | 18A19 | 1   | SCO2D27 | 266950 | 1038048968   | 15   | 321,00 | 337,95        |
| 69-01 | 18A19 | 1   | SCO2D27 | 266950 | 1038048968   | 15   | 321,00 | 337,95        |

---

## Passo 2 - Abrir o Protheus

1. Primeiro abriremos o Protheus, realizaremos o login com seu usuário e senha;
2. Confira os dados do sistema **Filial: 100103** | **Ambiente: 05 - Faturamento** se estiver tudo ok, clique em continuar;
3. Vamos acessar duas rotinas uma chamada **_Pedido de Venda_** e **_NFs-e_**;
4. Primeiro entre no **_Pedido de Venda_**, teremos uma tela com alguns pedidos iremos escolher o pedido

   > PEDIDO Nº: 000003 - PARA FROTAS PROPRIA
   > **Própria:** segue abaixo as placas referentes a frota própria;

   | TAG   | PLACA   | TRANSPORTADORA |
   | ----- | ------- | -------------- |
   | CB001 | SCO2D27 | STPLOG         |
   | CB002 | SCO2D37 | STPLOG         |
   | CB003 | SCO2D47 | STPLOG         |
   | CB004 | SCO2D57 | STPLOG         |
   | CB005 | SCO2D17 | STPLOG         |
   | CB006 | SCG6J48 | STPLOG         |
   | CB007 | SCG6F88 | STPLOG         |
   | CB008 | SCQ3C11 | STPLOG         |
   | CB009 | SCQ3B91 | STPLOG         |
   | CB010 | SCQ3C01 | STPLOG         |

   ***

   > PEDIDO Nº: 000008 - PARA FROTAS TERCEIRAS
   > **Terceiros:** segue abaixo as placas referentes a frota terceiros;

   | TAG   | PLACA   | TRANSPORTADORA |
   | ----- | ------- | -------------- |
   | LC012 | OXG0677 | BERALDO        |
   | LC015 | NYC3203 | BERALDO        |
   | LC017 | HMZ0886 | BERALDO        |
   | LC023 | HJH5060 | BERALDO        |
   | LC024 | HOB2886 | BERALDO        |

   ***

## Passo 3 - Configurando o pedido de venda

1. Com o veículo identificado e pedido de vendas conforme a frota, iremos alterar as informações do pedido para realizarmos o faturamento.
2. Clique em **`Alterar`**, será aberto uma tela com os parâmetros, precisamos se atentar à 5 parâmetros:

   - **Placa Veicul;**

     > **Note:** Onde iremos colocar a TAG ou a Placa do veículo, segue regra dos veículos cadastrados na tabela **`DA3`**;

   - **Mens.p/Nota;**

     > **Note:** Onde colocamos as informações recebidas por e-mail que são **`Nº FOLHA REG | PLACA`**;

   - **Prc Unitario;**

     > **Note:** Onde definimos o valor a tarifa do frete, que podemos saber utilizando a fórmula **`Preço com ICms / Peso`** dessa forma achamos o valor da tafira;

   - **Qtd Liberada;**

     > **Note:** Onde definimos o peso da carga informada no e-mail

   - **Classe de valor;**
     > **Note:** Onde definimos a classe de valor para os veículos de frota própria;
     > **OBS:** Não precisamos preencher este campo para frota de terceiros, basta preencher o campo **`Placa Veicul`**

3. Agora iremos preencher todos os campos mencionados acima, conforme a frota e dados enviados por e-mail;
4. Após preenchermos todos os dados necessários, podemos clicar em **`Salvar`**;
5. Após `Salvar` iremos acessar na mesma tela:
   > **`Outras Ações >> Prep.Doc.saída`**
6. Iremos clicar em **`Avançar >> Avançar >> Avançar >> Finalizar`**, na proxima tela selecione a opção **`RPS;`**

   > **Note:** Antes de avançar neste passo, precisamos conferir a sequência da nota no site ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)) e também na rotina **`NFs-e`** dentro do Protheus;

   > **Note:** Caso a sequência não esteja de acordo clique duas vezes na opção de **`RPS`** e modifique a numeração para ficar em sequência;

7. Se no Protheus e também no site estiverem de acordo a sequência numérica da nota podemos clicar em **`OK`**;
8. Depois teremos uma tela com outros parâmetros, sempre verifique se a opção **`Lanç.Contab.On-Line`** está como **`Não`** e pode clicar em **`OK`**;

---

## Passo 4 - Realizando transmissão

1. Após parametrizarmos a nota, iremos acessar novamente a rotina de **`NFs-e`**;
2. Nos parâmetros da rotina confira se **`Serie da nota fiscal`** está como **`RPS`** e a data podemos filtrar de um Mês antes até o hoje, depois podemos clicar em **`OK`**;
3. Vamos localizar a nota que geramos e realizaremos a transmissão da mesma
   > **Note:** Sempre confira o valor da nota gerada antes de realizar a transmissão, para evitar cancelamentos desnecessários tanto no sistema Protheus quanto no ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu));
4. Nota localizada iremos acessar nas opções: **`Outras Ações >> Transmissão`**;
5. teremos uma tela com os parâmetros de `Serie da nota, nota fiscal inicial e nota fiscal final`;
   - `Serie da nota:` sempre **RPS**;
   - `Nota fiscal inicial:` colocamos o número gerado para nossa nota;
   - `Nota fiscal final:` podemos deixar **_999999999_**, dessa forma o sistema intenderá que a partir da nota inicial até a nota final se tiver nota será transmitido;
6. Parametrizado os dados de transmissão iremos clicar em **`OK`** e aguarde a nota ser transmitida;
7. Após recebermos a mensagem que a nota foi transmitida podemos fazer o mesmo processo para o próximo veículo da planilha e realizar todo o procedimento novamente

---

> **Note:** Sempre que gerar uma nota, transmita ela após o termino pos se cadastrarmos uma outra nota o sistema pode quebrar a sequencia numérica da nota;

### Exemplo

No sistema temos uma tabela com duas colunas que precisam estar de acordo - **`NF Eletr.`** - númeração gerada pelo ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)) - **`Número`** - numeração gerada pelo Protheus.

| NF Eletr. | Número    |
| --------- | --------- |
| 100001212 | 100001212 |

---

## Passo 5 - Baixando as notas no NFe-Cidades

1. Primeiros acessamos o ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)), realizamos o login com o usuário e senha fornecidos;
2. No canto esquerdo teremos algumas opções iremos acessar a opção **`Solicitações`**;
3. Na próxima tela clique em **`Documentos emitidos`**;
4. Teremos alguns filtros modificaremos somente os de data conforme a data de geração da documentação;
5. Localize as notas geradas e baixe cada uma delas, para depois realizarmos o envio no e-mail;
