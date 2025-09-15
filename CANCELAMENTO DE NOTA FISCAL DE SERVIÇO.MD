# CANCELAMENTO DE NOTA FISCAL DE SERVIÇO -

---

## Passo 1 - Acessar a rotina `Exclusão de documentos de saída`

1. Ao acessar a rotina, verifique e ajuste, se necessário, os seguintes parâmetros:
   - `Data de emissão de`;
   - `Data de emissão até`;
   - `Série de`;
   - `Série até`;
2. A data deve ser filtrada conforme a data em que ela está sendo cancelada no sistema;
3. Defina a série como **`RPS`** para ambos os campos;
4. Após configurar os parâmetros, clique em **`OK`**;
5. Localize a nota fiscal desejada e selecione-a, em seguida, acesse:
   `Outras Ações >> Excluir`
6. Confirme o estorno da nota clicando em **`OK`**;
7. Na próxima tela, forneça o motivo do estorno e clique em **`OK`**;
8. Nas telas subsequentes, clique em **`OK`**, ignore quaisquer erros do sistema. Após o cancelamento, a nota fiscal será removida. Em seguida, acesse a rotina de  **`NFs-e`**;

---

## Passo 2 - Acessar a Rotina de Notas Fiscais Eletrônicas de Serviços (`NFs-e`) 

1. Nos parâmetros da rotina confira se **`Serie da nota fiscal`** está definida como **`RPS`** e a data podemos filtrar de um Mês antes até hoje, depois podemos clicar em **`OK`**;
2. Na tela inicial da rotina iremos acessar o menu:
    **`Outras Acções >> Cancelamento`**
    > **Note:** Caso a nota não apareca na tela precisamos realizar o monitoramento das notas emitidas para isso acesse na tela inical de **`NFs-e`** o menu:
    `Outras Ações >> Monitor`
3. Nos parâmetros de monitoramento, serão exibidos três campos
 - Série da nota fiscal: **`RPS`**
 - Nota fiscal inicial de: `Nota inical`
 - Nota fiscal final de : `Nota final`
4. Após definir os parâmetros, clique em **`OK`** Dependendo do intervalo de notas, o processo pode demorar alguns minutos.
   > **Note:** Ao acessar a rotina de **`NFs-e`** as notas com a marcação verde precisam ser monitoradas para garantir a comunicação com o sistema NF-e Cidades. Mantenha sempre as notas monitoradas;
5. Após o monitoramento das notas, retorne ao menu de cancelamento. Selecione a nota estornada e acesse o menu:
    **`Trans Canc`**  ou utilize o atalho **`T`**;
6. Após a transmissão, acesse o site do([NFe-cidades](https://www.nfe-cidades.com.br/landing-page)) para verificar se o cancelamento foi transmitido com sucesso;
