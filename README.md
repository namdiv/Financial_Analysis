# Análisis Financiero - S&P500

## Contexto
La empresa tomó la decisión de invertir parte de sus ganancias del año y va a tomar en cuenta el índice del SP500.
Este índice se basa en la capitalización bursátil de 500 grandes empresas que poseen acciones que cotizan en las bolsas NYSE o NASDAQ, y captura aproximadamente el 80% de toda la capitalización de mercado.

Luego del éxito que tuvo el informe ejecutivo y la normalización de datos del proyecto anterior, se solicitó al área de Datos ayuda con el análisis sobre los distintas empresas a lo largo del tiempo para comprender mejor el mercado, y poder tomar decisiones en base a nuestras recomendaciones.
Se trabajara con los periodos contemplados entre 01/01/2000 y 31/12/2021
Para este trabajo se utilizará la API de yahoo finance, cual posee su librería https://pypi.org/project/yfinance/ y página oficial https://finance.yahoo.com/
Los indicadores que se tomaron en cuenta fueron los siguientes:

- Cual es el mejor día para invertir teniendo en cuenta el retorno de los movimiento gap?
- Cual es el mejor día para invertir teniendo en cuenta el retorno de los movimientos intradiarios?
- Cuales son las mejores industrias que pertenecen al SP500 en las cuales se puede invertir?
- Cuales fueron los momentos de alta volatilidad que afectaron al SP500?
- Cuales son las 9 mejores empresas para invertir'

- retornos_gaps = np.log(aperturas/cierres.shift(1)).fillna(0)

- retornos_intra = np.log(cierres/aperturas).fillna(0)

- variaciones = activo.cierre_ajustado.pct_change()

- volatilidad = activos.variaciones.rolling(250).std()100(250)**0.5 (en este caso se puede utilizar el indice VIX)

Es necesario que determinen de manera gráfica dichos indicadores.

Por último, recuerden que los reportes que se desarrollarán serán para la toma de decisiones ejecutivas (Directores, vicepresidente y/o presidente de la empresa, etc), por lo tanto es imperativo evitar errores en los mismos.
