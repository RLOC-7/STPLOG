# EMISSÃO DE COMPLEMENTOS - PAINEL DE AGENDAMENTO

---

## Passo 1 - _Verificar informações no E-mail_

1. Abrir o e-mail (monitoramento.cbapocos@stplog.com.br).
2. Verificar caixa de entrada por **_( NFES_99-99-9999_NFES DE COMPLEMENTO_STPLOG )_**, neste e-mail contém todas as informações necessárias para à emissão dos CT-e de complemento
3. Manter o e-mail recebido aberto para cópia das informações.

---

## Passo 2 - _Abrir uma página em branco do Excel_

1. Copiar os dados do e-mail recebido;
2. Converter a planilha toda para texto;
3. Colar as informações na planilha utilizando **´(Ctrl + Shift + C)´** Pois realizando a colagem normal o Excel irá converter a numeração das chaves de acesso e não conseguiremos seguir no próximo passo;
4. Para melhor organização e agilidade de cadastro colocaremos um filtro no cabeçalho da Excel, para que ;possamos filtrar os veículos por **TAG** isso facilitará na hora de cadastrar;

---

### Exemplo

| MINA  | DMT   | TAG | PLACA   | NF     | CHAVE DE ACESSO                              | TONS  | PREÇO | PREÇO c/ ICMS |
| ----- | ----- | --- | ------- | ------ | -------------------------------------------- | ----- | ----- | ------------- |
| 32-53 | 20A21 | 1   | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69         |
| 32-53 | 20A21 | 1   | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69         |
| 32-53 | 20A21 | 1   | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69         |
| 32-53 | 20A21 | 1   | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69         |
| 32-53 | 20A21 | 1   | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69         |

---

## Passo 3 - _Realizar o download dos XML-S_

1. Primeiro vamos copiar uma **chave de acesso** e em seguida abrir o link ([Portal da Nota Fiscal Eletrônica](https://www.nfe.fazenda.gov.br/portal/consultaRecaptcha.aspx?tipoConsulta=resumo&tipoConteudo=7PhJ+gAVw2g=));
2. Após abrirmos o link iremos colar a **chave de acesso** copiada no campo **_Chave de Acesso da NF-e_**;
3. concorde com a _hCaptcha_;
4. Em seguida realizaremos a consulta clicando no botão **_CONTINUAR_**;
5. Será aberto uma nova tela, como iremos somente baixar clicaremos na opção de **_Download do documento_**;
6. Para melhor organização renomeei o arquivo XML para TAG do veículo mais o número posição dele na ordem;

---

### Exemplo

> CB001 - 1.xml
> CB001 - 2.xml
> CB001 - 3.xml

---

> **Note:** Dessa forma iremos ter os arquivos organizados na mesma ordem da planilha

---

## Passo 4 - Abrir o Protheus

1. Primeiro abriremos o Protheus, realize o login com seu usuário e senha;
2. Confira os dados do sistema **Filial: 100105** **Ambiente: 43 - TMS** se estiver tudo ok, clique em continuar;
3. Vamos acessar a rotina de **_Painel de Agendamento_**;
4. Teremos uma tela com alguns parâmetros iremos alterar somente a data para o dia de _Hoje_
5. Após entrar na tela da rotina escolhida teremos algumas abas em baixo clicar em **_Nfs Cliente_**;
6. Após selecionar **_Nfs Cliente_**, vamos clicar na opção quase no rodapé da página em **INCLUIR**;
7. Irá aparecer um cerregamento de código de barras podemos fechar, teremos a tela de _Cadastro de CT-e_;

---

## Passo 5 - Cadastro dos CT-e

- Teremos 8 Campos onde devemos ter bastante atenção na hora de preencher;
  - Codigo Veic;
  - Dev. Frete;
  - Serv.Transp;
  - Tipo Transp;
  - C.Custo Cred;
  - Selec.Origem;
  - Embalagem;

---

1.  Vamos colocar a TAG no campo de **_Codigo Veic_**;
    > **Note:** O sistema possui regras então se colocarmos uma TAG ou PLACA que não esteja no cadastro da tabela **DA3**, teremos o erro de "_Não existe registro relacionado a chave informada_";
2.  Clicamos em **_Outras Ações > Importar XML_** selecione o XML conforme a ordem feita na planilha;
    > **Note:** Atenção em selecionar os **XML**, para não confundir a ordem;
3.  Selecione o campo de **_Dev. Frete;_** escolha opção **_2 - Destinatário_**; Pode variar dependendo do frete;
4.  Quando selecionar vai ser avançado automaticamente para o campo de **_Serv.Transp;_** selecione opção **_3 - Entrega_**;
5.  De **TAB** uma vez e avançaremos para o campo de **_Tipo Transp;_** selecione opção **_1 - Rodoviário_**;
6.  Avance para o campo de **_C.Custo Cred;_**;

    > **Própria:** centro de custo sempre será **_203001 - TRANSP. ROM FROTA PROPRIA OFF ROAD_**, segue abaixo as placas referentes a frota própria;

    ***

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

    > **Terceiros:** centro de custo sempre será **_203004 - TRANSP. ROM FROTA TERCEIROS OFF ROAD_** segue abaixo as placas referentes a frota terceiros;

    | TAG   | PLACA   | TRANSPORTADORA |
    | ----- | ------- | -------------- |
    | LC012 | OXG0677 | BERALDO        |
    | LC015 | NYC3203 | BERALDO        |
    | LC017 | HMZ0886 | BERALDO        |
    | LC023 | HJH5060 | BERALDO        |
    | LC024 | HOB2886 | BERALDO        |

    ***

7.  Após identificar de qual frota o veículo pertence e parametrizar o centro de custo correto, avançamos para o campo de **_Selec.Origem;_**
8.  No campo de **_Selec.Origem;_** selecionamos a opção **_Cliente Remetente;_** Pode variar dependendo do frete. Avançamos para o campo de **_Embalagem;_**
9.  No campo de **_Embalagem_** iremos digitar **_GR_** que significa **_Granel_** pode variar de carga para carga, mas sempre trabalhamos com Granel;
10. Feito todo o processo podemos clicar em **_Salvar_** e passar para o próximo documento
    > **Note:** Ao terminar de **salvar** o sistema automaticamente irá abrir a tela de cadastro novamente é só aguardar alguns segundos para começar o próximo cadastro;

---

## Passo 6 | Ajuste da tabela de frete

1. Antes de realizar o calculo do CT-e precisamos verificar a o valor da tabela de frete para que possamos calcular os CT-e de acordo com os valores enviados pela **_CBA_**;
2. Abriremos uma nova rotina chamada **_Tab. Frete_**;
3. Para identificarmos nossa tabela correta, vamos se atentar a 4 colunas dentro do **_Protheus_**
   - Tab.Frete
   - Descricao
   - Reg.Origem
   - Reg.Destino
4. Vamos indentificar a linha que bater com os dados abaixo

| Tab.Frete | Descricao                          | Reg.Origem   | Reg.Destino     |
| --------- | ---------------------------------- | ------------ | --------------- |
| 0037      | FRETE PESO - CBA - POCOS DE CALDAS | DIVINOLANDIA | POCOS DE CALDAS |

5. Após localizar ela vamos clicar em **_Alterar_** ou atalho "a";
6. Com a nova tela aberta teremos duas abas **_Tabela de frete_** e **_Componentes de frete_**, vamos selelionar **_Componentes de frete_**;
7. Teremos uma tabela semelhante a tabela abaixo:
   | Item | Ate (Peso Mercadoria) | Fator Peso | Valor | Fracao | Comp. Tarifa |
   | - | - | - | - | - | - |
   | 01 | 999.999.999,999 | 999.999.999,999 | 30,52 | 1,0000 | Nao |
8. Iremos modificar somente o campo de **_Valor_**;
   > **Note:** Para chegar no valor correto do frete utilizamos uma formula básica dividir o valor total c/Icms pelo peso; Exemplo `PREÇO: 76,69 / PESO: 2,66 = 28,83`, dessa forma chegamos ao valor exato da tabela de frete.
9. Com o valor correto da tabela de Frete conferimos se já está ajustada caso não esteja realizamos o ajuste conforme a formula acima;

---

## Passo 7 - Realizando o calculo dos CT-e

1. Após configurar a Tabela de frete iremos retornar na rotina de **_Entrada documentos de clientes_**;
2. Vamos Localizar os documentos que cadastramos e iremos acessar **_Outras Acoes > Calculo de frete > Calcular_**;
3. Aparecerá uma tela informando que este processo tem como objetivo gerar documentos ficais clicaremos em **_OK_**;
4. Na próxima tela o sistema pergunta se desejamos informar o valor do frete manualmente, Como já configuramos a tabela de frete não necessita de informarmos manutalmente, podemos clilcar em **_Não_**;
5. Na próxima tela teremos as informações do calculo do frete, teremos uma tabela parecida com a da tabela de frete, confere os valores se tudo estiver de acordo podemos clicar em **_Confirmar_**;
6. iremos repetir o processo para todos os documentos em que cadastramos;

---

## Passo 8 - Puxando o PDF dos CT-e gerados pelo calculo de frete

1. Na mesma tela de **_Entrada documentos de clientes_** iremos acessar os itens abaixo:
   > Outras Acoes <-> Calculo de frete <-> CT-e
2. Teremos uma tela com os parametrôs da consulta, neste parte alteramos somente a data para o dia em que geramos os documentos, Caso a data já esteja de acordo podemos clicar em **_OK_**;
3. Aparecerá uma tabela com uma lista de CT-e gerados na data parametrizada;
4. Iremos Localizar os CT-e que geramos e clicaremos na coluna Documento no primeiro documento que geramos e vamos copiar os números utilizando o comando `Ctrl + C`, e a mesma coisa no ultimo documento gerado dos complementos;
5. Teremos algumas opções no rodapé do sistema localize a opção **_Dacte_** e clique nela;
6. Com os números de documentos copiados iremos colar eles nos campos de **_Documento De ?_** e **_Documento Até_** respeitando a ordem numérica gerada, depois de informar os números das documentações clicamos em **_OK_**;
7. Na próxima tela que aparecer pode clicar em **_OK_**;
8. O sistema irá perguntar se você deseja substituir o documente com o mesmo nome localizado na pasta onde está sendo salvo, pode clicar em **_SIM_**;
9. Após salvaremos o arquivo gerado em uma pasta separada na área de trabalho;
   > **Dica:** Renomeei o arquivo para `CT-e 00009999 - 00009999`, número inicial do documento e número final do documento gerado, pois pode facilitar na hora de pesquisar no e-mail;
