# Tecnologias de Transmissão de Dados em Sistemas Web

## Módulo 1 - Descrever a linguagem de marcação XML e sua aplicabilidade em sistemas web
### Linguagem XML
* Parecida com HTML mas para outros fins.
* Utilizada para transmissão de dados, onde o programador escolhe a tag que quiser transmitir os dados, assim o receptor de seu XML vai conseguir utilizar o mesmo padrão que você criou para conseguir ler os dados de acordo.
### Anatomia de um arquivo XML
* Geralmente os XML são compostos por dados em String, onde existe a marcação e dentro dessa marcação ocorre o valor em si.
```xml
<? xml version="1.0" enconding="UTF-8" ?>
<correntistas>
  <!-- Nesse documento há dados de duas 'pessoas' -->
  <pessoa>
    <tipo>física</tipo>
    <nome>José Maria</nome>
    <numero>000.00-00</numero>
  </pessoa>

  <pessoa>
    <tipo>jurídica</tipo>
    <nome>José Maria SA</nome>
    <numero>111.11-11</numero>
  </pessoa>
</correntistas>
```
* 1 linha é a declaração do xml, responsável por especificar a versão e informar ao navegador que se trata de um arquivo XML, além de definir o charset do documento.
* 2 linha, representado pela tag <correntistas> é o nó principal, ou nó raiz. 
* 3 linha primeiro elemento filho do nó raiz o elemento <pessoa>
* 4, 5, 6 linha temos os elementos filhos do elemento <pessoa>
* Levando em consideração a organização do XML, podemos destacar que é um arquivo bem formatada.
### Utilizando Atributos
```xml
<?xml version="1.0" encoding="UTF-8" ?>
<correntistas>
  <conta agencia="0123-4">
    <tipo>física</tipo>
    <nome>José Maria</nome>
    <numero>000.000-00</numero>
  </conta>
  <conta agencia="5678-9">
    <tipo>jurpidica</tipo>
    <nome>José Maria SA</nome>
    <numero>111.111-11</numero>
  </conta>
</correntistas>
```
* Podemos utilizar esse tipo de formatação mostrada acima ou então esse tipo de formatação abaixo
```xml
<?xml version="1.0" encoding="UTF-8"?>
<correntistas>
  <conta agencia="0123-4" tipo="física" nome="José Maria" numero="000.000-00" />
  <conta agencia="5678-9" tipo="jurídica" nome="José Maria SA" numero="111.111-11" />
</correntistas>
```
1. XML é autodocumentado, ou seja, seu formato descreve sua estrutura, elementos e valores.
2. XML é independente de plataforma e linguagem de programação.
3. XML é facilmente interpretado pela maioria das linguages de programação.
4. XML é extensível. Logo, podemos tanto usar entidades criadas por outros, quanto criar nossas próprias tags e atributos.
5. XML possui suporte a Unicode.
6. XML possui suporte à validação através de DTD e Schema.
* Desvantagens
1. XML não suporta Arrays.
2. XML pode gerar arquivos grandes dada a sua sintaxe detalhada.
### Manipulando um arquivo XML com a interface DOM.
* É possível manipular XML usando Javascript facilmente, esse método é chamadado de XML DOM 
---
## Módulo 2 - 