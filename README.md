# Lojas_N3xt
Lojas_N3xt
<h1> Vinculação com inventario <h1>

<h2> Primeira Etapa </h2>

Para Vincular o nosso resource ao inventario Primeiramente você Precisa fazer as alterações no inventario.

<b>Essa Vinculação é necessaria então não pule nenhuma etapa!</b>

<h3>Etapa 01 Vinculação no Meta</h3>

Dentro da Pasta do Seu Inventario localiza o Arquivo "meta.xml"

<img src='https://i.imgur.com/ZF1xvW1.png'>

Após Localizado Abra o mesmo e dirija-se até o final do codigo

<img src='https://i.imgur.com/Wlqteer.png'>

Aqui você Vai colocar a seguinte Linha:

	'<export function="getInventoryItems" type="server" />'
  
Lembre-se de colocar no final do codigo, antes do fechamento do meta, como a imagem exemplo abaixo:

<img src='https://i.imgur.com/AP6X0aS.png'>

> Adicionado essa Linha vamos agora para etapa 2 

<h2> Segunda Etapa </h2>

Localize nos Arquivos do inventario o script Config

<img src='https://i.imgur.com/Fr69ma0.png'>

Abra o mesmo e desça até o final dele

<img src='https://i.imgur.com/qTRRN46.png'>

No final do seu codigo vc vai adicionar a seguinte função:

function getInventoryItems()
   return config.itens
end

segue o exemplo a baixo

<img src='https://i.imgur.com/oOOitk4.png'>

Terminamos aqui por enquanto a vinculação dos dois scripts, vamos ensinar agora como criar lojas

<h2> Criação de Lojas </h2>

Para A Criação de lojas é simples, Abra o Arquivo do script RSC_n3xt_lojas e procure o arquivo RSC_Config.lua

<img src='https://i.imgur.com/kWZp32D.png'>

Dentro do Arquivo você vai encontrar a seguinte linha de codigo:

<img src='https://i.imgur.com/UaomUQ6.png'>

Esse Bloco de Codigo que vc vai Utilizar para Criar Sua Loja 

o Numero entre [ ] Corresponde a Numeração da loja

<img src='https://i.imgur.com/uJTxycb.png'>

Em seguida temos o nome da Loja (Pode ser qualquer nome, o mesmo será usado dnv)

<img src='https://i.imgur.com/lh7y1yV.png'>

e logo abaixo temos os dados para configuração de Posição

<img src='https://i.imgur.com/DcQRBUK.png'>

Sendo {Pos X, Pos Y, Pos Z}

logo em seguida temos as Cores

<img src='https://i.imgur.com/Vuz0jG5.png'>

Sendo { Cor R, Cor G, Cor B}

Logo em seguida temos Opacidade e Tamanho:
<img src='https://i.imgur.com/0oolGNe.png'>

Para Criação Basta Copiar todo o bloco de codigo que vimos agora 

<img src='https://i.imgur.com/XGIJQrX.png'>

E Logar em Baixo do ' }, '

<img src='https://i.imgur.com/AUpnR6e.png'>

Após isso devemos obrigatoriamente mudar o numero da loja seguindo a ordem (isso é muito importante não pode haver numero repetitos ou pular algum numero)

<img src='https://i.imgur.com/V70TI9i.png'>

Após isso basta configura os dados como gostaria com nome da loja podendo sim ser repetido, Posição do marker, Cor, Tamanho e Opacidade.

Agora Vamos Configurar para que os itens apareçam na loja

<h2> Terceira Etapa </h2>

Após realizar todas as configurações no arquivo de Lojas, o restante é no inventario então volte para o inventario e abra novamente o arquivo config

<img src='https://i.imgur.com/Fr69ma0.png'>

Abra ele Novamente so que dessa vez vamos modificar os itens, Vamos adicionar nas linhas dos itens a informação ' loja ' dessa forma:

<img src='https://i.imgur.com/K9LzQ22.png'>

estamos fazendo no ultimo item para que você entenda melhor.

Agora você vai definir qual loja esse item vai aparecer, no nosso caso vamos coloca na 'farmacia' para teste apenas.

<img src='https://i.imgur.com/4Ru3ibI.png'>

logo após temos que verificar se na linha ja possui a informação de ' valor = PREÇO ' e 'desc = DESCRIÇÃO' caso não tenha vamos adicionar, nessa linha não temos nenhuma das duas então iremos adicionar:

<img src='https://i.imgur.com/3GhFZSS.png'>

A Ordem não importa com tanto que todas as informações estejam presente, agora so fazer isso para todos os itens determinando loja = "nome da loja" que o item vai aparecer valor e descrição

OBS: o nome do inventario deve ser 'n3xt_inventario' não pode mudar para que o script funcione corretamente




