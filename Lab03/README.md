## Lab03 - Model-View-Controller
### Orquestração e Coreografia<br>
Manoel Teixeira<br><br>
## Tarefa 1 - Diagrama de Orquestração

![Diagrama de Orquestração](images/Inf331Lab03Tarefa1MTDCeDA.GIF)
<br>

## Tarefa 2 - Diagrama de Coreografia
![Diagrama de Coreografia](images/Tarefa2.JPG) </br>

Sequencia dos Passos, referente ao Diagrama de Coreografia

</br>a) Tudo começa pela Interface A, onde através desta o cliente manifesta o seu desejo de adquirir um produto no Marketplace, via o componente selecionar produto; 
</br>b) A partir da Interface B se busca o produto escolhido, ou seja, que por sua vez será entregue ao componente lança cotação;
</br>c) Na sequencia, via a interface C, a cotação é lançada no barramento, por evento, onde os fornecedores subscritos, através de categoria de produto, poderão participar desta transação;
</br>d) Ai, começa, efetivamente a disputa pelos fornecedores, pois cada um deles vai colocar o seu melhor preço naquele produto e retornar no barramento;
</br>e) Finalmente, a Interface Z, via o componente pega os três melhores preços, ou seja, os menores, a fim de devolver ao cliente, a fim de proceder com a sua escolha.</br>

## Tarefa 3
Seguem as telas do meu aplicativo "Tarefa 3 - Prototipo de Compras":
<br><table border="0"><tr><td>Tela 1 <br>Nenhum produto selecionado<br><img alt="Tela 1 - nenhum produto selecionado" 
src="images/Tela01.jpeg" width="60%" height="35%" /></td><td>Tela 2<br>Primeiro produto selecionado <br><img 
alt="Tela 2 - primeiro produto selecionado" src="images/Tela02.jpeg" width="60%" height="35%" /></td> </tr><tr> <td> Tela 3 <br>Segundo produto selecionado <br><img 
alt="Tela 3 - segundo produto selecionado" src="images/Tela03.jpeg" width="60%" height="35%" /></td><td> Tela 4 <br>Compra de um dos produtos efetiva<br><img 
alt="Tela 4 <br>Compra de um dos produtos efetiva" src="images/Tela04.jpeg" width="60%" height="35%" /></td><td>  
</td><td>  </td></tr></table>

<b> Diagrama de blocos do aplicativo</b>
<br><br><img alt="Diagrama de blocos do aplicativo" src="images/Inf331Lab03Tarefa3MT ImagensDosBlocos.png" width="50%" height="50%" /><br>
  
[Baixe aqui o arquivo do aplicativo exportado a partir do MIT App Inventor em formato aia.](app/Inf331Lab03Tarefa3MT.aia)<br>
   
## Tarefa 4
Imagens da Equipe 4 postadas no endereço [https://github.com/grupo04](https://github.com/grupo04)
