[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"
![valid XHTML][checkmark]

[getcomposer]: https://getcomposer.org/
[uninstall-mods]: https://getcomposer.org/doc/03-cli.md#remove
[artigo-composer]: http://mozg.com.br/ubuntu/composer
[ioncube-loader]: http://www.ioncube.com/loaders.php
[acordo]: http://mozg.com.br/acordo-licenca-usuario-final/

# Mozg\MagentoLocale

## Sinopse

Pacote de traduçao pt_BR

Toda a estrutura é baseada nos arquivos nativo en_US

Foi aproveitada a tradução do pacote do MarioSam e para registros que não tinha tradução foi usado mecanismo para tradução automática

## Testando na Heroku

Gostaria de apresentar o aplicativo que disponibilizei para a plataforma Heroku

Com apenas 1 clique, o aplicativo cria sua loja virtual usando a plataforma de comércio eletrônico Magento e instala os módulos da MOZG

[https://github.com/mozgbrasil/heroku-magento#descrição](https://github.com/mozgbrasil/heroku-magento#descrição)

## Instalação - Atualização - Desinstalação

--

Este módulo destina-se a ser instalado usando o [Composer][getcomposer]

Execute o seguinte comando no terminal, para visualizar a existencia do Composer e sua versão

	composer --version

Caso não tenha o Composer em seu ambiente, sugiro ler o seguinte artigo [Clique aqui][artigo-composer]

--

Sugiro manter um ambiente de testes para efeito de testes e somente após os devidos testes aplicar os devidos procedimento no ambiente de produção

--

Sugiro efetuar backup da plataforma Magento e do banco de dados

--

Antes de efetuar qualquer atualização no Magento sempre mantenha o Compiler e o Cache desativado

--

Certique se da presença do arquivo composer.json na raiz do seu projeto Magento e que o mesmo tenha os parâmetros semelhantes ao modelo JSON abaixo

	{
	  "minimum-stability": "dev",
	  "prefer-stable": true,
	  "license": [
	    "proprietary"
	  ],
	  "repositories": [
	    {
	      "type": "composer",
	      "url": "https://packages.firegento.com"
	    }
	  ],
	  "extra": {
	    "magento-root-dir": "./",
	    "magento-deploystrategy": "copy",
	    "magento-force": true
	  }
	}

Caso não exista o arquivo composer.json na raiz do projeto Magento, crie o mesmo adicionado o conteúdo acima

### Para instalar o módulo execute o comando a seguir no terminal do seu servidor

    composer require mozgbrasil/magento-locale-pt_br

--

### Para atualizar o módulo execute o comando a seguir no terminal do seu servidor

    composer update

--

### Para [desinstalar][uninstall-mods] o módulo execute o comando a seguir no terminal do seu servidor

    composer remove mozgbrasil/magento-locale-pt_br

## Perguntas mais frequentes "FAQ"



## Badges

[![Join the chat at https://gitter.im/mozgbrasil](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/mozgbrasil/)
[![Latest Stable Version](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/v/stable)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![Total Downloads](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/downloads)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![Latest Unstable Version](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/v/unstable)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![License](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/license)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![Monthly Downloads](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/d/monthly)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![Daily Downloads](https://poser.pugx.org/mozgbrasil/magento-locale-pt_br/d/daily)](https://packagist.org/packages/mozgbrasil/magento-locale-pt_br)
[![Reference Status](https://www.versioneye.com/php/mozgbrasil:magento-locale-pt_br/reference_badge.svg?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:magento-locale-pt_br/references)
[![Dependency Status](https://www.versioneye.com/php/mozgbrasil:magento-locale-pt_br/1.0.0/badge?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:magento-locale-pt_br/1.0.0)

:cat2:
