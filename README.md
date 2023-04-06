# Classificação - Taxa de Cancelamento de Reservas de Hotéis

## Data Science Project - Taxa de Cancelamento de Reservas de Hotéis

![Hotel_01](https://user-images.githubusercontent.com/104601836/230490095-52a95967-0a34-4306-a0e3-e8510de8ca6f.jpg)


# 1. Problema do Negócio
A Costa del Data (empresa fictícia) é uma tradicional rede hoteleira espanhola. Ela possui hoje hotéis de 4 e 5 estrelas em todo o território nacional.
A empresa está preocupada com as suas projeções para os próximos anos, visando a recuperação financeira com o fim das restrições impostas pela pandemia de Covid-19.
Com a reabertura das fronteiras, a diminuição nas restrições de viagem e o aumento das vacinações, era esperado que o setor hoteleiro da Espanha retomasse os ganhos outrora esperados.
Na contramão desta expectativa, a Costa del Data tem visto um aumento em sua taxa de cancelamentos de reservas! A suspeita da diretoria é de que houve uma mudança no comportamento de cancelamentos por parte do consumidor após a pandemia, que ainda não foi compreendida pela rede.
Isso travou ações estratégicas críticas como a expansão da rede hoteleira, a reforma das unidades já com obras programadas, e a realização de ações de marketing direcionadas.

# 2. Premissas do Negócio
Foram desconsiderados fatores recentes como: conflitos armados, aumento de preços energéticos, acordos comerciais e aprovações orçamentárias que envolvam a Espanha, Europa e o mundo como um todo.

# 3. Estratégia da Solução
O modelo foi desenvolvido com utilização de dos seguintes Algoritmos de Classificação: XGBoost, Gradient Boosting e Random Forest.
Após implementação dos algoritmos, foi realizado um comparativo entre os três com a geração da moda e posterior avaliação do melhor valor a ser considerado na projeção.

# 4. Insights de Dados
A taxa de cancelamento de reserva nos Hotéis 4 Estrelas é de 41,6%, enquanto nos Hotéis de 5 Estrelas a taxa de cancelamento cai para 28%.
Para o regime de alimentação completa (Café da manhã, Almoço e Jantar), considerando as duas classes de hotel, a taxa de cancelamento é de aproximadamente 60%, enquanto nos demais regimes de alimentação (Sem Refeição, Café da Manhã e Café da Manhã e Jantar) a taxa de cancelamento fica entre 34% e 38%.
As reservas feitas diretas no balcão tendem a ter uma taxa de cancelamento menor do que as reservas feitas por empresas e agências de turismo, sendo 17%, contra 22% e 41%, respectivamente.
Os hóspedes que já se hospedaram anteriormente possuem uma taxa de cancelamento menor em hotéis da rede, sendo 15% comparado à taxa de 38% dos que ainda não se hospedaram.
Considerando as reservas de hospedagem feitas com inclusão de vaga no estacionamento, não houve cancelamento nestas.
Reservas com mais de 3 de observações possuem menor taxa de cancelamento comparado às reservas sem nenhuma, ou até 3 observações, sendo 8,4%, contra 48% e 22%, respectivamente.

# 5. Produto Final
Com base no histórico de reservas dos hóspedes, foi desenvolvido um modelo de previsão de cancelamentos, o qual visa prever a variável alvo "Reserva Cancelada", retornando 1 em caso de cancelamento, e 0 em caso de não cancelamento.

# 6. Conclusão
O objetivo do projeto foi desenvolver um modelo de previsão de cancelamentos que visa compreender este fenômeno.
Em posse dos resultados, o time de marketing poderá tomar decisões mais assertivas, focando nos públicos com menor incidência de cancelamento, revertendo assim o cenário negativo atual.
Com a implementação do modelo, foi possível prever a taxa de cancelamentos com uma eficácia de 97%, ou seja, entre 100 registros com dados de clientes, o modelo pode prever a possibilidade de cancelamento de até 97 registros com exatidão.
Traduzindo em valores, tendo como premissa que o preço médio de uma diária de hotéis entre 4 e 5 estrelas seja € 300 e possua um total de 250 quartos disponíveis, pode-se calcular um faturamento mensal de € 2.250.000 (Diária x Qtd. Quartos x 30 dias) em caso de ocupação máxima. Desta forma, considerando que 37% das reservas eram canceladas antes da aplicação do modelo, pode-se calcular um prejuízo de € 832.500.
Tendo como base uma lotação de 80% dos quartos disponíveis, aplicando o modelo com eficácia aproximada de 97%, pode-se concluir uma economia de aproximadamente € 646.000, somando anualmente aproximadamente € 7.750.000.
Observação: Para este cálculo foi considerado: 97% (assertividade do modelo) x € 832.500 (faturamento perdido por cancelamento) x 80% (estimativa de ocupação).


# 7. Próximos Passos
Como próximos passos serão definidos estudos detalhados sobre as características dos clientes de modo isolado, permitindo que a equipe de Marketing possa focar em cada tipo de público considerando suas particularidades e, assim, definir uma estratégia mais assertiva.

