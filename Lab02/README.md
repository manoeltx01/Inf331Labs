## Lab02 - Data Flow e Messages
## ALUNO
   Manoel Teixeira
<br><br> 
## 1	Tarefa sobre catalogo de componenetes

 [Link para o NOTEBOOK das tarefas] (notebook/components-01-catalog.ipynb)

## 2	Tarefa Web Componentes 1
~~~htlm
<dcc-trigger label="Mundo"
             action="noticia/mundo/politica"
             value="A crise entre os Chines e os EUA não tem fim!">
</dcc-trigger>
<dcc-trigger label="Brasil P"
             action="noticia/brasil/politica"
             value="Um Páis do falso moralismo">
</dcc-trigger>
<dcc-trigger label="Brasil E"
             action="noticia/brasil/esporte"
             value="Ja foi o melhor do mundo em futebol?">
</dcc-trigger>
<dcc-trigger label="Bahia"
             action="noticia/bahia/esporte"
             value="Uma das paixões dos baianos é o futebol">
</dcc-trigger>

<dcc-lively-talk duration="0s"
                 character="doctor"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/+/politica"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk duration="0s"
                 character="nurse"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/brasil/#"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk duration="0s"
                 character="patient"
                 speech="I heard about a ">
  <subscribe-dcc topic="noticia/#"></subscribe-dcc>
</dcc-lively-talk>
~~~


## 3 Tarefa Web Componentes 2

```html
<dcc-trigger label="Science New Item" action="next/rss">
</dcc-trigger>

<dcc-rss publish="rss/science" source="https://www.wired.com/category/science/feed">
<subscribe-dcc topic="next/rss" role="step"></subscribe-dcc>
</dcc-rss>

<dcc-trigger label="Design New Item" action="next2/rss2">
</dcc-trigger>

<dcc-rss publish="rss/design" source="https://www.wired.com/category/design/feed">
<subscribe-dcc topic="next2/rss2" role="step"></subscribe-dcc>
</dcc-rss>

<dcc-aggregator publish="aggregate/science" quantity="3">
<subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-aggregator>


<dcc-lively-talk id="doctor"
                 duration="0s"
                 character="doctor"
                 speech="News ">
  <subscribe-dcc topic="aggregate/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="nurse"
                 duration="0s"
                 character="nurse"
                 speech="News ">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="patient"
                 duration="0s"
                 character="patient"
                 speech="News ">
  <subscribe-dcc topic="rss/design"></subscribe-dcc>
</dcc-lively-talk>
```




