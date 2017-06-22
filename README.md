# tamanhos-da-ufcg

Temos 3 arquivos vindos do dump de abril dos dados abertos do governo federal sobre seus servidores, publicados no portal de transparência do governo federal:

**ufcg-201704-tudo.csv** tem todos os dados do cadastro dos servidores no governo federal. (Não incluímos vencimentos nem observações, que são distribuídos em arquivos diferentes)

**ufcg-201704-unidades-academicas-filtradas.csv** contém apenas informações de pessoal nas Unidades Acadêmicas da UFCG, excluindo pessoal de administração nos Centros. Também possui menos colunas, focando no que provavelmente é de interesse para alguém analisando apenas a UFCG.

**ufcg-201704-sumario-UAs-wide.csv** contém um exemplo de sumário calculado a partir de `ufcg-201704-unidades-academicas-filtradas.csv`. As colunas são:
* `UORG_LOTACAO` Unidade acadêmica de lotação do funcionário   
* `Outro` Número de funcionários na UA que não são professores   
* `Professor 20h` Número de professores com carga horária 20h/semana na UA   
* `Professor 40h ou DE` Número de professores com carga horária 40h/semana na UA, sejam eles Dedicação Exclusiva ou não   
* `idade_25perc`, `idade_mediana` e `idade_75perc` : 25, 50 e 75 percentil da idade dos funcionários *no cargo* (ex: idade_25perc = 10 significa que 25% dos funcionários, sejam eles professores ou não, da UA tem 10 anos ou menos na profissão.)   
