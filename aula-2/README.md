# Pipeline de Dados sobre criptomoedas

Objetivo é desenvolver um pipeline de dados para a análise de sentimento de notícias relacionadas ao Bitcoin usando dados obtidos da [API Alpha Vantage](https://www.alphavantage.co/documentation/) através do parâmetro **function=NEWS_SENTIMENT** na chamada da API, que retorna informações de sentimento de notícias.

Para fazer a chamada à API foram definidos alguns parâmetros para retornar os dados desejados, como:

**function=NEWS_SENTIMENT** -  que retorna informações de sentimento de notícias.

**tickers=CRYPTO:BTC'** - especifica o ticker do ativo financeiro que deseja ser analisado. Neste caso, "CRYPTO:BTC", indicando que análises de sentimento de notícias relacionadas ao Bitcoin estão sendo solicitadas.

Além de outros parâmetros utilizados que ficam a critério da quantidade de informações desejada.

**time_from** - define a data e hora inicial para se trazer informações solicitadas sobre as notícias;

**limit** - número máximo de notícias retornadas;

-------------------------------

Os dados extraídos passam por todo processo de pipeline desde a extração e transformação até serem disponibilizados com as informações finais para consumo. Para isso os dados, a pipeline foi dividida em camadas __bronze__, __silver__ e __gold__.