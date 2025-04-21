# Limpeza de Dados com Python
<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">

🔧 Etapas da Limpeza Realizadas
1. Padronização de Tipos e Formatos

    Datas:

        Todas as datas foram convertidas para o formato YYYY-MM-DD.

    Horas:

        Horários convertidos para o padrão HH:MM:SS.

    Valores Numéricos:

        As colunas valor, quantidade, frete e total foram convertidas para tipo numérico (float ou int).

        Valores com símbolos (ex: "R$", ",") foram limpos para manter apenas os números com . como separador decimal.

        Importação da biblioteca (re) para facilitar na limpeza de caracteres nas colunas.

2. Tratamento de Inconsistências

    Valores Ausentes:

        Registros com campos essenciais ausentes (ex: valor, quantidade) foram removidos.

        Dados faltantes não essenciais foram preenchidos com estratégias específicas (ex: frete com média, datas com modo).

    Registros Duplicados:

        Foram identificados e removidos X registros duplicados, mantendo apenas a versão mais recente ou completa.

    Verificação de Cálculo do Total:

        Aplicada a fórmula:
        total = valor * quantidade + frete

        Registros com cálculos incorretos foram corrigidos

    Tratamento do nome do Vendedor:

        Conforme vimos, há uma inconsistência em relação ao nome dos vendedores. Nesse caso, colocamos eles como DESCONHECIDO ao realizar a limpeza..
