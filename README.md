# Tweepy
En el programa mostrado, se aplica un código que se conecta a la API de Twitter y extrae los Tweets que contienen la palabra buscada. Esto se puede hacer por localidad, idioma, coordenadas, fechas, depende de lo se indica al programa. 
La finalidad de esta aplicación, es darle un formato útil y analizable a los tweets extraídos, que se descargan en formato json y se transforman a una tabla de Excel por comodidad didáctica. 

En "Tweepy_muy_bueno.ipynb" está el código desarrollado que se conecta a la API y que le da el formato de excel a los tweets.

En el excel "muymalo.xlsx" están los tweets con la búsqueda de palabras clave "muy malo".

En el excel "malo.xlsx" están los tweets con la búsqueda de palabras clave "malo".

En el excel "bueno.xlsx" están los tweets con la búsqueda de palabras clave "bueno".

En el excel "muybueno.xlsx" están los tweets con la búsqueda de palabras clave "muy bueno".

En el excel "Excelente.xlsx" están los tweets con la búsqueda de palabras clave "excelente" y "perfecto".

El archivo "Grafico_de_sentimientos.ipynb" es un programa que grafica la "positividad o negatividad" de la temática extraída. Lo que hace es abrir un archivo en donde se guarda la información extraída desde el módulo "Extractor_de_datos_de_twitter". Dentro de ese extractor se guardan los datos en un archivo csv."twitter-out.csv"

El módulo "Medidor_de_sentimientos" muestra como se puntuan los tweets.

Luego en el programa "Modulo_del_medidor_de_sentimientos" se entrenan los modelos "SGDClassifier", "LinearSVC_classifier", "LogisticRegression_classifier", "BernoulliNB_classifier", "MNB_classifier", "originalnaivebayes" con los archivos "positive.txt" y "negative.txt". Y se crea una función en la que cada comentario pasado por todos estos clasificadores, selecciona el mejor modelo que puntúa el tweet.
