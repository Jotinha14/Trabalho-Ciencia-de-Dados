
# Limpeza de Dados com Python
## <p align="center"><strong><span style="color:blue;">Relatório Resumido</span></strong></p>

Etapas da Limpeza de Dados:
Datas:
Todas as datas foram padronizadas no formato internacional AAAA-MM-DD, facilitando a organização e a leitura dos registros.

Horários:
Os horários foram ajustados para o modelo de 24 horas, no formato HH:MM:SS, garantindo consistência nas análises envolvendo tempo.

Valores Numéricos:
As colunas com valores monetários e quantitativos como valor, quantidade, frete e total. Depois foram convertidas para tipos numéricos adequados (float ou int).

Durante esse processo, foram removidos símbolos como “R$” e vírgulas, adotando o ponto (.) como separador decimal. Para facilitar essa limpeza, utilizamos expressões regulares com a biblioteca re.

Tratamento de Dados Incompletos ou Duplicados:
Campos Vazios
Registros com informações essenciais faltando, como valor ou quantidade, foram removidos.
Já os campos que não comprometem a integridade dos dados foram preenchidos com estratégias específicas. Por exemplo, o frete foi substituído pela média dos valores existentes, e datas ausentes foram preenchidas com o valor mais frequente (moda).

Registros Duplicados:
Também foi feita uma verificação de duplicatas. Um total de X registros repetidos foi identificado e excluído, priorizando sempre a versão mais completa ou mais recente.

Correção do Campo "Total":
Para garantir que os valores do campo total estavam corretos, aplicamos a fórmula-padrão:

python
Copiar
Editar
total = (valor * quantidade) + frete
Quando identificamos divergências, os valores foram recalculados e atualizados com base nessa regra.
# Trabalho-Ciencia-de-Dados

