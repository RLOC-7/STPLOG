# EMISSÃO DE COMPLEMENTOS - ENTRADA DOCUMENTOS DE CLIENTE
---
## Passo 1 - *Verificar informações no E-mail*
1. Abrir o e-mail (monitoramento.cbapocos@stplog.com.br).
2.  Verificar caixa de entrada por **_( NFES_99-99-9999_NFES DE COMPLEMENTO_STPLOG )_**, neste e-mail contém todas as informações necessárias para à emissão dos CT-e de complemento
3. Manter o e-mail recebido aberto para cópia das informações.
---
## Passo 2 - *Abrir uma página em branco do Excel*
1. Copiar os dados do e-mail recebido;
2. Converter a planilha toda para texto;
3. Colar as informações na planilha utilizando **´(Ctrl + Shift + C)´** Pois realizando a colagem normal o Excel irá converter a numeração das chaves de acesso e não conseguiremos seguir no próximo passo;
4. Para melhor organização e agilidade de cadastro colocaremos um filtro no cabeçalho da Excel, para que ;possamos filtrar os veículos por **TAG** isso facilitará na hora de cadastrar;
---
###  Exemplo

| MINA | DMT | TAG | PLACA | NF | CHAVE DE ACESSO | TONS | PREÇO | PREÇO c/ ICMS |
|------|-----|-----|-------|----|-----------------|------|-------|---------------|
| 32-53 | 20A21 | 1 | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69 |
| 32-53 | 20A21 | 1 | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69 |
| 32-53 | 20A21 | 1 | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69 |
| 32-53 | 20A21 | 1 | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69 |
| 32-53 | 20A21 | 1 | SCO2D27 | 266950 | 35240361409892021413550000002669501716463400 | 2,660 | 67,48 | 76,69 |
---

## Passo 3 - *Realizar o download dos XML-S*
1. Primeiro vamos copiar uma **chave de acesso** e em seguida abrir o link ([Portal da Nota Fiscal Eletrônica](https://www.nfe.fazenda.gov.br/portal/consultaRecaptcha.aspx?tipoConsulta=resumo&tipoConteudo=7PhJ+gAVw2g=));
2. Após abrirmos o link iremos colar a **chave de acesso** copiada no campo ***Chave de Acesso da NF-e***;
3. concorde com a *hCaptcha*;
4. Em seguida realizaremos a consulta clicando no botão ***CONTINUAR***;
5. Será aberto uma nova tela, como iremos somente baixar clicaremos na opção de ***Download do documento***;
6. Para melhor organização renomeei o arquivo XML para TAG do veículo mais o número posição dele na ordem;
---
### Exemplo
> CB001 - 1.xml
> CB001 - 2.xml
> CB001 - 3.xml
---
> **Note:** Dessa forma iremos ter os arquivos organizados na mesma ordem da planilha 
---
## Passo 4 - Abrir o Protheus e criação de LOTES 
1. Primeiro abriremos o Protheus realiza o login com seu usuário e senha;
2. Confira os dados da sistema **Filial: 100105** **Ambiente: 43 - TMS** se estiver tudo ok, clique em continuar;
3. Vamos acessar a rotina de *Entrada documentos de clientes*;
4. Após entrar na tela da rotina escolhida iremos clicar em ***INCLUIR***  ou atalho *i*;
5. Acessando a nova tela iremos procurar por *No.Lote** e clicaremos na lupa;
6. Vamos ter uma tela onde podemos realizar consulta de Lotes e criação de novos, vamos clicar em **INCLUIR**;
7. Na tela de entrada de lotes, iremos alterar somente dois parâmetros ;
	- *Qtd.Lote:* sempre a quantidade **1**;
	- *Tipo Lote:* sempre **3 - Eletrônico**;
8. Após parametrizar os campos clicaremos em ***Salvar e Criar Novo*** assim conseguimos criar o próximo lote;
9. Criado todos os lotes necessários seguimos para o **Passo 5 - Cadastar os CT-e**;
10. Feche todas as telas de Lote e fique na tela de cadastro do CT-e *(Doctos. Do Cliente para Transporte)*;
---
> **Note:** Na criação dos lotes, criamos todos os lotes necessários para o cadastros dos CT-e, por exemplo se recebemos **15 CT-e** criamos **15 Lotes**, dessa forma ajuda a manter a ordem dos cadastros dos CT-e e caso chegue outros **CT-e** referentes as rodadas diárias conseguimos retomar do lote que criamos mantendo a ordem do cadastro ;

> **Dica:** Quando realizar o cadastro do primeiro Lote pegue o número dele e adicione em uma coluna do Excel que criamos, no Excel a célula onde colocamos o número vai ter um quadrado pequeno e verde no canto direito em baixo, clique e segure e arraste até a ultima célula dos **CT-e**  para que ele forneça uma ordem numérica os lotes, isso irá facilitar o cadastro, pois podemos copiar o número dos lotes direto da planilha;
---
## Passo 5 - Cadastro dos CT-e
 - Teremos 8 Campos onde devemos ter bastante atenção na hora de preencher;
	> No.Lote;
	> Codigo Veic;
	> Dev. Frete;
	> Serv.Transp;
	> Tipo Transp;
	> C.Custo Cred;
	> Selec.Origem;
	> Embalagem;
---
 1. iremos pegar o primeiro Lote e colar no campo ***No.Lote;***
 2. Vamos colocar a TAG no campo de ***Codigo Veic***;
	 > **Note:** O sistema possui regras então se colocarmos uma TAG ou PLACA que não esteja no cadastro da tabela **DA3**, teremos o erro de "*Não existe registro relacionado a chave informada*";
	 
 3. Clicamos em ***Outras Ações > Importar XML*** selecione o XML conforme a ordem feita na planilha;
	 > **Note:** Atenção em selecionar os **XML**, para não confundir a ordem;
 4.  Selecione o campo de ***Dev. Frete;*** escolha opção ***2 - Destinatário***; Pode variar dependendo do frete;
 5. Quando selecionar vai ser avançado automaticamente para o campo de ***Serv.Transp;*** selecione opção ***3 - Entrega***;
 6. De **TAB** uma vez e avançaremos para o campo de ***Tipo Transp;*** selecione opção ***1 - Rodoviário***;
 7. Avance para o campo de ***C.Custo Cred;***;
	 > **Própria:**	centro de custo sempre será ***203001 - TRANSP. ROM FROTA PROPRIA OFF ROAD***, segue abaixo as placas referentes a frota própria;
    ---
    | TAG   | PLACA   | TRANSPORTADORA |
    |------ | ------- | -------------- |
	| CB001 | SCO2D27 |     STPLOG     |
	| CB002 | SCO2D37 |     STPLOG     | 
	| CB003 | SCO2D47 |     STPLOG     | 
	| CB004 | SCO2D57 |     STPLOG     | 
	| CB005 | SCO2D17 |     STPLOG     | 
	| CB006 | SCG6J48 |     STPLOG     | 
	| CB007 | SCG6F88 |     STPLOG     | 
	| CB008 | SCQ3C11 |     STPLOG     | 
	| CB009 | SCQ3B91 |     STPLOG     | 
	| CB010 | SCQ3C01 |     STPLOG     | 
	
    ---
	 > **Terceiros:** centro de custo sempre será ***203004 - TRANSP. ROM FROTA TERCEIROS OFF ROAD*** segue abaixo as placas referentes a frota terceiros;
	
    | TAG   | PLACA   | TRANSPORTADORA | 
    |------ | ------- | -------------- | 
    | LC012 | OXG0677 | BERALDO        |
    | LC015 | NYC3203 | BERALDO        |
    | LC017 | HMZ0886 | BERALDO        |
    | LC023 | HJH5060 | BERALDO        |
    | LC024 | HOB2886 | BERALDO        |

	--- 
 8. Após identificar de qual frota o veículo pertence e parametrizar o centro de custo correto, avançamos para o campo de ***Selec.Origem;***
 9. No campo de ***Selec.Origem;*** selecionamos a opção ***Cliente Remetente;*** Pode variar dependendo do frete. Avançamos para o campo de ***Embalagem;***
 10. No campo de ***Embalagem*** iremos digitar ***GR*** que significa ***Granel*** pode variar de carga para carga, mas sempre trabalhamos com Granel;
 11. Feito todo o processo podemos clicar em ***Salvar*** e passar para o próximo documento
     > **Note:** Ao terminar de **salvar** o sistema automaticamente irá abrir a tela de cadastro novamente é só aguardar alguns segundos para começar o próximo cadastro;
---
## Passo 6 | Realizando o Calculo dos CT-e

1. Antes de realizar o calculo do CT-e precisamos verificar a o valor da tabela de frete para que possamos calcular os CT-e de acordo com os valores enviados pela ***CBA***;
2. Abriremos uma nova rotina chamada ***Tab. Frete***