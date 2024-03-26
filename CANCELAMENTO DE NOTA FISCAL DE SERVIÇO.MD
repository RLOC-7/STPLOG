# CANCELAMENTO DE NOTA FISCAL DE SERVIÇO -

---

## Passo 1 - Acessar a rotina `Exclusão de documentos de saída`

1. Quando entrar na rotina irá aparecer alguns parametrôs, teremos que modificar alguns campos se não estiverem de acordo que são:
   - `Data de emissão de`;
   - `Data de emissão até`;
   - `Série de`;
   - `Série até`;
2. A data filtramos no dia que fizemos a emissão do documento;
3. Nos dois compos da série coloque **`RPS`**;
4. Depois de configurado os parametros podemos seguir clicando em **`OK`**;
5. Localize a nota fiscal lançada, Localizada e selecionada iremos acessar:
   `Outras Ações >> Excluir`
6. Irá aparecer se queremos realmente realizar o estorno da nota, podemos Clicar em **`OK`**;
7. Na proxima tela vamos ter um campo para informar o motivo do estorno, informe o motivo e clique em **`OK`**;
8. Nas proximas telas podemos clicar em **`OK`**, pois são algums erros do sistema logo após nossa nota fiscal irá desaparecer, e assim que ela sumir iremos acessar a rotina de **`NFs-e`**;

---

## Passo 2 - Acessar a rotina `NFs-e`

1. Nos parâmetros da rotina confira se **`Serie da nota fiscal`** está como **`RPS`** e a data podemos filtrar de um Mês antes até hoje, depois podemos clicar em **`OK`**;
2. Na tela inicial da rotina iremos acessar o menu:
    **`Outras Acções >> Cancelamento`**
    > **Note:** Caso a nota não apareca na tela precisamos realizar o monitoramento das notas emitidas para isso acesse na tela inical de **`NFs-e`** o menu:
    `Outras Ações >> Monitor`
3. Nos parametros teremos apenas três campos
 - Serie da nota fiscal: **`RPS`**
 - Nota fiscal inicial de: `Nota inical`
 - Nota fiscal final de : `Nota final`
4. Clique em **`OK`** dependendo do intervalo de notas pode demorar alguns minutos;
   > **Note:** Quando acessar a rotina de **`NFs-e`** as notas que estiverem com a bolinha verde precisam ser monitoradas para que haja comunicação com NF-e Cidades, sempre mantenha monitorado as notas;
5. com as notas monitoradas podemos voltar no menu de cancelamento, iremos selecionar nossa nota que estornamos e vamos acessar o menu:
    **`Trans Canc`** ou atalho **`T`**;
6. Logo após a transmissão ser realizada podemos acessar o site do ([NFe-cidades](https://www.nfe-cidades.com.br/home/inicial-menu)), e conferir se o cancelamento foi transmitido com sucesso para o site também;