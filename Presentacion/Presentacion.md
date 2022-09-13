---
marp: true
theme: default
paginate: true
---

# Trabajo Práctico N°2: Finanzas 
# Vidman Xavier Harry

---

# Obtención de los datos de cada empresa

## Comenzamos obteniendo los símbolos de cada empresa a través de la URL de wikipedia: https://en.wikipedia.org/wiki/List_of_S%26P_500_companies

---
# Descargamos todos los datos de cada empresa, en formato .csv, de la database de Yahoo Finance. 

# Luego se concatenan para crear un solo DataFrame con toda la información
---
# DataFrame de las empresas de S&P500

![sp500](Img/sp500_img1.PNG)

---
# Calculamos los índices financieros y los agregamos como columnas al dataframe

![sp500_img2](Img/sp500_img2.PNG)

---

# ¿Cuál es el mejor día para invertir teniendo en cuenta el retorno de los movimientos gap?¿Y el movimiento intradiario?

---

# Graficos de los días de la semana

![grafico1](Img/dias_mean_volume.PNG)    ![grafico2](Img/dias_sum_volume.PNG)

---

# Graficamos la media del "Retorno de gap" para cada día de la semana. Vemos que el mejor día es el MARTES

![grafico3](Img/dias_gap_return.PNG)

---

# Graficamos la media del "Retorno intradiario" para cada día de la semana. Vemos que el mejor día es el JUEVES

![grafico3](Img/dias_intra_return.PNG)

---

# ¿Cuáles son las mejores industrias que pertenecen al S&P500 en las cuales se puede invertir?

![grafico_industrias](Img/industrias.PNG)

---

# Retorno medio de gap de cada industria

![grafico_gap_ind](Img/industrias_gap_return.PNG)

---

# Mejores industrias: "Retorno intradiario" y "Retorno Gap", de media, POSITIVOS. 

## Consumer Discretionary 
## Health Care Industry 
## Industrials 
## Information Technology


---

# Retorno medio intradiario de cada industria

![grafico_gap_ind](Img/industrias_intra_return.PNG)

---

# ¿Cuáles son las 9 mejores empresas para invertir?
## Sumamos las columnas del DataFrame, agrupando por Symbol y Year

![grafico](Img/df_symb_per_year.PNG)

---

# Calculamos la diferencia entre los Retornos del 2021 y 2020

![grafico](Img/pendientes.PNG)

---

# Filtramos las mejores empresas con pendiente_gap y pendiente_intra

## Luego, nos quedamos con las 9 de mayor volumen

![grafico](Img/top10_companies.PNG)

---

# Fin
# ¡Muchas Gracias!
