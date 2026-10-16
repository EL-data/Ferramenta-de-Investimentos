# Ferramenta-de-Investimentos
Atividade desenvolvida na formação de analise de dados com excel e ia da DIO
O projeto foi desenvolvido para responder as seguintes perguntas de negócio:
"Quanto dinheiro eu deveria investir com base no meu salário?" Essa pergunta tem a resposta encontrada com facilidade como "sugestão de investimento" atravéz do calculo de 30% do salario informado. 
"Quanto terei de patrimonio em Y anos se investir mensalmente X valor?" Essa resposta aparece nomeada como Patrimonio acumulado e é gerada após informar o valor de investimento mensal recorrente (Aporte) e o tempo decorrido.
"Quanto terei de patrimonio acumulado em 5,10,15,20,30,40 e 50 anos?" Essas respostas são calculadas automaticamente a partir da informação de aporte e podem ser encontradas em uma tabele chamada "Cenários"
"Qual será o meu dividendo mensal para cada valor de patrimonio?" A responta para essa pergunta pode ser encontrada em dois momentos diferentes. Juntamente com os valores de patrimonio pré definidos e no campo "Dividendos mensais" que corresponde aos dividendos recebidos à partir do patrimonio acumulado em Y anos. Sendo o valor de Y informado pelo usuario no campo especificado da ferramenta.
"Qual porcentagem do meu dinheiro investir em cada tipo de FII de acordo com meu perfil de investidor?" Para ajudar com isso há uma tabela nomeada de sugestão de carteira, nela são mostradas 6 categorias de FIIs e há um campo onde o usuário pode selecionar seu perfil de investidor e a parti dessa informação a tabela retorna uma sugestão de distribuição do aporte mensal entre essas categorias. 

Para realizar os cálculos do valor de patrimonio acumulado foi utilizada a fórmula "=VF(Taxa;Tempo*12;Aporte*-1)". Substituindo-se tempo pelo numero de anos especificado nas opções pré-cálculadas.

Para cria a Tabela de sugestão de carteira foi necessarios criar uma tabela de apoio e com o uso da formula (=PROCV(Perfil&"-"&[Categoria de fundo];Planilha2!A3:D21;4;FALSO)" para conseguir introduzir o valor percentual recomendado à cada perfil de investidor. Para facilitar a criação das formulas as categorias de fundos foram organizadas numa coluna à esqueda da coluna com o percentual de investimento associado, de forma que nas formulas dentro da ferramente categoria de fundo estará referenciada como uma célula onde estará descrito o nome da categoria fundo imobiliario correspondente.  

Foram criados os seguintes intrervalos nomeados: Aporte(E16);Dividendos(E20);Patrimonio(E19);Perfil(I12);Taxa(E12);Tempo(E17);Salário(E13)

<img width="437" height="387" alt="image" src="https://github.com/user-attachments/assets/9d2022b8-ddc3-4c77-8b37-d352db5a2ca1" />
Na imagem acima estão visiveis os valores utlizados como recomendação de investimento. São valores estipulados por mim mesmo com base em pesquisas à documentos de recomendação de investimento e relatórios de balanço de diferentes instituições financeiras. Usei os relatório de ago/2026, set/2026 e out/2026 da Xp investimentos, Itaú, Inter e recomendações da Empiricus para basear minhas inferencias.

Fiz a ferramenta bem similar à que o expert demonstrou fazendo apenas algumas pequenas alterações como esquema de cores, Valores de sugestão de investimento e a adição de gráficos na ferramenta.

<img width="1280" height="759" alt="Captura_Ferramenta_FII_3" src="https://github.com/user-attachments/assets/60c3dcc0-f335-44be-92a2-1b8848af4ccb" />
<img width="1280" height="763" alt="Captura_Ferramenta_FII_2" src="https://github.com/user-attachments/assets/879bc550-1216-4c67-9b19-f8128656eadc" />
<img width="1280" height="761" alt="Captura_Ferramenta_FII_1" src="https://github.com/user-attachments/assets/21cea5b9-bdbb-4d06-b34d-71df73d07f35" />
<img width="1280" height="758" alt="Captura_Ferramenta_FII_4" src="https://github.com/user-attachments/assets/61fc75d4-4931-43b0-8aa6-e695273fbaa9" />


[Ferramenta_de_investimento_com_FIIS.xlsx](https://github.com/user-attachments/files/33579084/Ferramenta_de_investimento_com_FIIS.xlsx)
