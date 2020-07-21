# Bases legais do LGPD


## Características

  - Bases legais do LGPD
  - Mudança de paradigma e hipótese de justificativa
  - Não há nenhuma hierarquia, ocorre para fins casualistas
  - Artigo 7º Hipótese para dados não sensíveis

## Pontos de Destaques Dados Não Sensíveis
  - [Consentimento](README.md###consentimento)
  - Execução de políticas públicas
  - Realização de Estudo e pesquisa
  - Leis e agencias regulatórias
  - Execução de contrato
  - Protecao da vida
  - Tutelação da saúde
  - Interesse legítimo
  - Proteção de Crédito

### Consentimento  
 - É mais difundido e conhecido
 - O detentor dos dados pode escolher ou não ser pode haver interferência
 - Deve ser evidente e clara e não ambígua
 - É vetado o  seu uso genérico
 - Precisa ter uma finalidade, deve ter avisado quando ocorrer alguma mudança
 - Deve ser escrito ou por outro meio  e deve ser explícito
 - Devem ser documentados
 - Como fica o consentimento de criança, seja passou por responsável?

### Execução de políticas públicas
-	Realizados por órgãos públicos
-	Utilizados em caso de segurança pública ou defesa nacional
-	Sistema de monitoramento inteligente (SIM), realizar a Geocalização em blocos (anomização)
-	Ser para fins públicos e sem disponibilizar para terceiros.
-	Garantir a segurança caso haja vazamento
-	Não limitar o tempo de uso de dados

### Realização de Estudo e pesquisa

-	Dados anomizados
-	Intenção de votos para eleição

### Leis e agencias regulatórias
-	Obrigações legais da CLT, os dados não subordinam ao empregado.
-	Nicho regulatório, e.x. da ANVISA, prática farmacêutica, dados do responsável, farmacêutico e do médico.
-	SAC  sequencia numérica para identificar o chamado. Obrigatoriedade de manter a gravação por 90 dias. icam 2 anos depois da solução do chamado.

### Execução de contrato
-	Contratação do serviço da NET, quando é necessário  cumprir as obrigações como endereço, assim como o e-commerce, procedimento preliminares, também como instituições financeiras.

### Proteção da vida

-	Tem que ser específica
-	Não pode ser aplicada genericamente
-	Consulta de dados por geocalização para uma pessoa desaparecida ou se for soterrada

### Tutelação da saúde
-	Possuir um plano de Mitigação do risco
-	Triagem ou checagem na emergência ou no atendimento hospitalar

### Interesse legítimo
-	O contrate usa para fins concretos
-	Uso de dados estritos e transparente
-	E o impacto desses dados
-	Interesse e legítimo da união europeia
-	Etapas do interesse de legitimidade

#### Legitimidade de interesse
-	Necessidade
-	Balanceamento – o interesse está subpondo o direito do detentor?
-	Salvaguardas – transparência, documentação, válvula de escape, maleável

### Proteção de Crédito

-	Dados de inadimplência serão usados para fornecimento de crédito
-	A proteção de crédito não tem na GPDR, oriundo do contexto brasileiro
-	Atrelado a análise de dados por algoritmo
-	O detentor pode solicitar a revisão


## Pontos de Destaques Dados  Sensíveis

- Consetimento – forma destacada e específica
- TO DO
- TO DO
- TO DO
- TO DO

### Prevenção de fraude
-	Utilizado para acesso a locais restritos, transação financeira por instituições bancárias 
-	Prevenção de fraude – é indispensável para autenticação e confirmação de identidade por meio de dados biométricos ou genéticos
-	É resguarda sob o artigo 9º
-	Não podem prevalecer sobre os direitos fundamentais




Markdown is a lightweight markup language based on the formatting conventions that people naturally use in email.  As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

### Tech

Dillinger uses a number of open source projects to work properly:

* [AngularJS] - HTML enhanced for web apps!
* [Ace Editor] - awesome web-based text editor
* [markdown-it] - Markdown parser done right. Fast and easy to extend.
* [Twitter Bootstrap] - great UI boilerplate for modern web apps
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework [@tjholowaychuk]
* [Gulp] - the streaming build system
* [Breakdance](https://breakdance.github.io/breakdance/) - HTML to Markdown converter
* [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

### Installation

Dillinger requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
