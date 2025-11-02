|Identificador  |UC-01 - Selecionar Andar                              |
|---------------|------------------------------------------------------|
|Função         |Permite ao hospede selecionar o andar desejado        |
|Atores         |Hospede                                               |
|Pré Condição   |Nenhuma                                               |
|Pós Condição   |O andar é selecionado                                 |
|Fluxo Principal|1. Hóspede seleciona o andar na botoeira externa<br> 2. Botoeira informa qual elevador irá buscar o hóspede|

|Identificador    |UC-02 - Realizar reconhecimento facial                           |
|-----------------|-----------------------------------------------------------------|
|Função           |Permite ao hospede fazer o reconhecimento facial para andares VIP|
|Atores           |Hospede                                                          |
|Pré Condição     |O andar selecionado ser da categoria VIP                         |
|Pós Condição     |O rosto da pessoa é escaneado e autorizado para o andar          |
|Fluxo Principal  |1. Hóspede seleciona o andar VIP na botoeira externa<br> 2. Botoeira informa qual elevador irá buscar o hóspede<br> 3. Elevador chega no andar VIP<br> 4. Elevador faz o reconhecimento facial antes de abrir a porta<br> 5. O rosto é validado<br> 6. O elevador abre as portas|
|Fluxo Alternativo|1. Hóspede seleciona o andar VIP na botoeira externa<br> 2. Botoeira informa qual elevador irá buscar o hóspede<br> 3. Elevador chega no andar VIP<br> 4. Elevador faz o reconhecimento facial antes de abrir a porta<br> 5. O rosto é recusado|

|Identificador  |UC-03 - Verificar o uso do elevador                           |
|---------------|--------------------------------------------------------------|
|Função         |Permite ao gerente conferir as câmeras internas dos elevadores|
|Atores         |Gerente Unidade                                               |
|Pré Condição   |Gerente da Unidade estar logado no sistema                    |
|Pós Condição   |O gerente fez a verificação do uso do elevador                |
|Fluxo Principal|1. Gerente acessa o sistema<br> 2. Gerente abre as cameras do elevador|

|Identificador  |UC-04 - Cadastrar categorias de andar                                     |
|---------------|--------------------------------------------------------------------------|
|Função         |Permite ao gerente selecionar quais serão os andares VIP e quais os Comuns|
|Atores         |Gerente Unidade                                                           |
|Pré Condição   |Gerente da Unidade estar logado no sistema                                |
|Pós Condição   |Um novo andar é adicionado categoria VIP                                  |
|Fluxo Principal|1. Gerente do sistema seleciona o andar<br> 2. Gerente do sistema seleciona a categoria do andar|

|Identificador  |UC-05 - Dimensionar elevadores                                      |
|---------------|--------------------------------------------------------------------|
|Função         |Permite ao gerente escolher quais elevadores atenderão quais andares|
|Atores         |Gerente Unidade                                                     |
|Pré Condição   |Gerente da Unidade estar logado no sistema                          |
|Pós Condição   |Os andares contemplados pelos elevadores são atualizados            |
|Fluxo Principal|1. Gerente do sistema seleciona o elevador<br> 2. Gerente do sistema seleciona os andares que o elevador vai contemplar|

|Identificador      |UC-06 - Gerenciar gerentes das unidades                                                |
|-------------------|---------------------------------------------------------------------------------------|
|Função             |Permite ao usuário master criar, excluir ou editar os acessos dos gerentes das unidades|
|Atores             |Usuário Master                                                                         |
|Pré Condição       |1. Usuário master estar logado no sistema|
|Pós Condição       |1. O acesso de um gerente de unidade é inserido<br> 2. O acesso de um gerente de unidade é alterado<br> 3. O acesso de um gerente de unidade é removido|
|Fluxo Principal    |1. O Usuário Master cria um novo usuário<br> O Usuário Master seleciona o tipo de acesso do novo usuário|
|Fluxo Alternativo 1|1. O Usuário Master seleciona um usuário<br> O Usuário Master seleciona o novo tipo de acesso do usuário|
|Fluxo Alternativo 2|1. O Usuário Master seleciona um usuário<br> O Usuário Master remove o usuário         |


|Identificador  |UC-07 - Acionar alarme de incêncio                            |
|---------------|--------------------------------------------------------------|
|Função         |Permite ao gerente acionar o alarme de incêncio dos elevadores|
|Atores         |Gerente Unidade                                               |
|Pré Condição   |Gerente da unidade estar logado no sistema                    |
|Pós Condição   |Elevadores vão para o térreo                                  |
|Fluxo Principal|1. Gerente da unidade aperta o alarme de incêndio<br> 2. Todos os elevadores vão para o térreo e abrem as portas|

|Identificador  |UC-08 - Acionar alarme de emergência                            |
|---------------|----------------------------------------------------------------|
|Função         |Permite ao gerente acionar o alarme de emergência dos elevadores|
|Atores         |Gerente Unidade                                                 |
|Pré Condição   |Gerente da unidade estar logado no sistema                      |
|Pós Condição   |Elevadores ficam fechados e parados no andar mais próximo       |
|Fluxo Principal|1. Gerente da unidade aperta o alarme de emergência<br> 2. Todos os elevadores vão para o andar mais próximo e abrem as portas<br> 3. Quando todos saírem os elevadores fecham as portas|

|Identificador  |UC-09 - Cadastrar facial                                                                  |
|---------------|------------------------------------------------------------------------------------------|
|Função         |Permite ao sistema de CheckIn enviar as informações de faciais cadastradas para o elevador|
|Atores         |Sistema CheckIn                                                                           |
|Pré Condição   |O hóspede estar hospedado no hotel                                                        |
|Pós Condição   |O rosto foi adicionado ao sistema do elevador                                             |
|Fluxo Principal|1. O hóspede faz checkin no hotel<br> 2. O hóspede cadastra a facial no sistema do hotel<br> 3. O sistema do hotel envia a facial para o sistema do elevador|