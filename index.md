---
layout: slide
---
<section data-markdown><script type="text/template">

{% include iftech_logo.html %}

# My kid Api
### Criando uma Rest API com Django e Python

<br>
[Renato César Lira Borges](https://github.com/rencesar)

29 de Novembro de 2018

</script></section>

<section data-markdown><script type="text/template">

## O que iremos abordar?

1. Teorica
    * O que são Rest APIs
    * Metodos HTTP
    * Como desenhar uma Rest API
    * Autenticação
2. Pratica
    * Setup Django Rest Framework
    * Criando `Serializers`
    * Criando meu primeiro `Endpoint`
    * Vamos Autenticar

</script></section>

<section data-markdown><script type="text/template">

## BUT WAIT!!
<img class="plain" width=50% src={{ "/images/whoareyou.gif" | prepend: site.baseurl }}>

</script></section>

<section data-markdown><script type="text/template">

## Quem sou eu

Renato César, Desenvolvedor de Software a mais de 2 anos.
Atualmente trabalho remotamente para [Broadsheet](https://www.broadsheet.com.au/) e curso Sistemas para Internet no IFPB.

</script></section>

<section data-markdown><script type="text/template">

## REST API?!
<img class="plain" width=50% src={{ "/images/masoqeisso.jpg" | prepend: site.baseurl }}>

</script></section>

<section data-markdown><script type="text/template">
### Representational State Transfer (REST)

Funciona como um comunicador entre qualquer aplicação e seu backend.

<img class="plain" width=40% src={{ "/images/rest-api-1.png" | prepend: site.baseurl }}>

</script></section>

<section data-markdown><script type="text/template">
## Para que serve
<br>
Para possibilitar uma comunicação entre diferentes streams (frameworks/linguagens), exemplo: 

* Aplicação movel (java)
* Front-end  (React)
* Back-end (Python)

</script></section>

<section data-markdown><script type="text/template">

## Como funciona

1. Cliente faz uma `request` `GET` para `myapi.com/movies/`
2. Servidor recebe requisição
3. Vai ao banco de dados pega os filmes
4. Retorna os filmes em `JSON` `response HTTP 200 (OK)`

</script></section>

<section data-markdown><script type="text/template">

## HTTP códigos

<img class="plain" width=70% src={{ "/images/http-codes.jpg" | prepend: site.baseurl }}>


</script></section>

<section data-markdown><script type="text/template">

## HTTP methods

<table>
    <tbody>
        <tr>
            <td>GET</td>
            <td>O método `GET` solicita a representação de um recurso específico.</td>
        </tr>
        <tr>
            <td>HEAD</td>
            <td> Idêntica ao método `GET`, porém sem conter o corpo da resposta.</td>
        </tr>
        <tr>
            <td>POST</td>
            <td>Utilizado para submeter uma entidade a um recurso específico.</td>
        </tr>
        <tr>
            <td>PUT</td>
            <td>O método `PUT` substitui dados de um objeto atual por outros.</td>
        </tr>
        <tr>
            <td>DELETE</td>
            <td>O método `DELETE` remove um recurso específico.</td>
        </tr>
        <tr>
            <td>PATCH</td>
            <td>O método `PATCH` é utilizado para aplicar modificações parciais em um recurso.</td>
        </tr>
    </tbody>
</table>


</script></section>

<section data-markdown><script type="text/template">

## Endpoints

<img class="plain" width=70% src={{ "/images/endpoint.png" | prepend: site.baseurl }}>


</script></section>

<section data-markdown><script type="text/template">

## Autenticação vs Autorização

1. Autenticação

    * Verificar credenciais (login)
    * Verificar se você é você

2. Autorização

    * Verificar se com certas credenciais contem autorização de acesso



</script></section>

<section data-markdown><script type="text/template">

## Tipos de Autenticações

1. [Basic Authentication](https://tools.ietf.org/html/rfc2617)
2. [HMAC (hash based message authentication)](https://tools.ietf.org/html/rfc2617)
3. [OAuth](https://tools.ietf.org/html/rfc6749)


click nos links e sera redirecinado para as RFCs

</script></section>

<section data-markdown><script type="text/template">

# Let's CODE!

<img class="plain" width=70% src={{ "/images/letscode.gif" | prepend: site.baseurl }}>

</script></section>

<section data-markdown><script type="text/template">

# Set up

1. Clone repositorio: `https://github.com/rencesar/supermarket-djangoapi-tutorial`
2. Siga os passos do `README.MD`
3. As próximas instruções serão dadas na apresentação

</script></section>

<section data-markdown><script type="text/template">

## Referencias e materiais extras

* https://www.django-rest-framework.org/
* https://blog.restcase.com/restful-api-authentication-basics/
* https://tableless.com.br/entendendo-tokens-jwt/
* https://testdriven.io/dockerizing-django-with-postgres-gunicorn-and-nginx
* https://www.getpostman.com/
* https://medium.com/@marcosrabaioli/django-rest-framework-e-django-oauth-toolkit-c71f8920db08

</script></section>
<section data-markdown><script type="text/template">

## Renato César

[Github](https://github.com/rencesar)

[LinkedIn](https://linkedin.com/in/renatocesarlira/)

</script></section>
