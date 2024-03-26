# EMISSÃO DE NOTAS FISCAIS DE SERVIÇO -
---
## Passo 1 - Verificar informações no E-mail {#Passo1}

1. Abrir o e-mail (monitoramento.cbapocos@stplog.com.br).
2. Verificar caixa de entrada o e-mail recebido parecido com **_(Viagens Terceiros - Mês 2024)_**, neste e-mail contém todas as informações necessárias para à emissão da NF-e
3. Manter o e-mail recebido aberto para cópia das informações.

### Exemplo de como as informações chega no e-mail

`Por gentileza, emitir as NF’s dos seguintes serviços:`
`Locação Caminhão Pipa (PC 4516926488/20 | FRS 1038168122): R$49.269,220`
`Transportes Diversos (PC 4516926488/10 | FRS 1038168158): R$841,750`

---

## Passo 2 - Abrir o Protheus {#Passo2}

1. Primeiro abriremos o Protheus, realizaremos o login com seu usuário e senha;
2. Confira os dados do sistema **Filial: 100103** | **Ambiente: 05 - Faturamento** se estiver tudo ok, clique em continuar;
3. Vamos acessar duas rotinas uma chamada **_Pedido de Venda_** e **_NFs-e_**;
4. Primeiro entre no **_Pedido de Venda_**, teremos uma tela com alguns pedidos iremos escolher o pedido:
   **`TRANSPORTE DIVERSOS Nº: 000007`**

## Passo 3 - Abrir o Excel para conversão {#Passo3}

1. Vamos abrir uma planilha do Excel em branco, com as informações do e-mail iremos adicionar algumas no excel;
2. em cada celula separada iremos adicionar:

- `Valor total do serviço`;
- `Tarifa do frete`;

### Exemplo de como descobrir as horas do serviço prestado:
> **Note:** A tarifa é de `R$ 194,74` por hora, então para calcular quantas horas de serviço foram prestadas para alcançar o valor total de `R$ 841,75`, você divide o valor total pela tarifa por hora

`Número de horas = Valor total / Tarifa por hora`
`= 841,75 / 194,74`
`≈ 4,32 horas`

> **OBS:** Com o valor das horas descoberto podemos pegar a mesma fórmula acima e no excel a celula que vai realizar a fórmula convertemos para valor em reais e adicionamos 6 casas depois da vírgula para ficar conforme o campo **`Qtd Liberada`** no Protheus e assim teremos o resultado para termos o valor total do serviço no sistema;

## Passo 4 - Configurando o pedido de venda {#Passo4}

1. Com o pedido de vendas conforme o serviço, iremos alterar as informações do pedido para realizarmos o faturamento.
2. Clique em **`Alterar`**, será aberto uma tela com os parâmetros, precisamos se atentar à 3 parâmetros:

   - **Mens.p/Nota;**

     > **Note:** Onde colocamos as informações recebidas por e-mail que são **`Nº FOLHA REG | PC - Pedido de Compra`**;

   - **Prc Unitario;**

     > **Note:** Onde definimos o valor da tarifa do frete, informada por e-mail `RS 194,74`;

   - **Qtd Liberada;**

     > **Note:** Onde definimos a quantidade em horas convertida em valor, realizada no [Passo 3](#Passo3)


3. Agora iremos preencher todos os campos mencionados acima, com os dados que fizemos a conversão e os dados do e-mail;
4. Após preenchermos todos os dados necessários, podemos clicar em **`Salvar`**;
5. Após `Salvar` iremos acessar na mesma tela:
   > **`Outras Ações >> Prep.Doc.saída`**
6. Iremos clicar em **`Avançar >> Avançar >> Avançar >> Finalizar`**, na proxima tela selecione a opção **`RPS;`**

   > **Note:** Antes de avançar neste passo, precisamos conferir a sequência da nota no site ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)) e também na rotina **`NFs-e`** dentro do Protheus;

   > **Note:** Caso a sequência não esteja de acordo clique duas vezes na opção de **`RPS`** e modifique a numeração para ficar em sequência;

7. Se no Protheus e também no site estiverem de acordo a sequência numérica da nota podemos clicar em **`OK`**;
8. Depois teremos uma tela com outros parâmetros, sempre verifique se a opção **`Lanç.Contab.On-Line`** está como **`Não`** e pode clicar em **`OK`**;

---

## Passo 5 - Realizando transmissão {#Passo5}

1. Após parametrizarmos a nota, iremos acessar novamente a rotina de **`NFs-e`**;
2. Nos parâmetros da rotina confira se **`Serie da nota fiscal`** está como **`RPS`** e a data podemos filtrar de um Mês antes até hoje, depois podemos clicar em **`OK`**;
3. Vamos localizar a nota que geramos e realizaremos a transmissão da mesma;
   > **Note:** Sempre confira o valor da nota gerada antes de realizar a transmissão, para evitar cancelamentos desnecessários tanto no sistema Protheus quanto no ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu));
4. Nota localizada iremos acessar nas opções: **`Outras Ações >> Transmissão`**;
5. teremos uma tela com os parâmetros de `Serie da nota | nota fiscal inicial | nota fiscal final`;
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

## Passo 6 - Baixando as notas no NFe-Cidades {#Passo6}

1. Primeiros acessamos o ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)), realizamos o login com o usuário e senha fornecidos;
2. No canto esquerdo teremos algumas opções iremos acessar a opção **`Solicitações`**;
3. Na próxima tela clique em **`Documentos emitidos`**;
4. Teremos alguns filtros modificaremos somente os de data conforme a data de geração da documentação;
5. Localize as notas geradas e baixe cada uma delas, para depois realizarmos o envio no e-mail;
