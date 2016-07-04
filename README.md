[EN]
# PHP 5.6 + MongoDB Driver (legacy) + Apache 

This modified DIY cartridge provides PHP 5.6.23 with MongoDB Driver (legacy), and fully free Apache configuration permission, which can be found in `conf` folder.

## Quick Start

[![Click to install OpenShift](http://launch-shifter.rhcloud.com/launch/light/Click to install.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=diy-0.1&initial_git_url=https://github.com/LucasPadilha/openshift-php-apache.git&name=php)

1. Open https://openshift.redhat.com/app/console/application_type/cart!diy-0.1 
2. Fill **Source Code** text field: `https://github.com/LucasPadilha/openshift-php-apache.git`
3. Click **Create Application** and wait
4. Open your website (e.g. foo-bar.rhcloud.com ) and keep your browser running. Meanwhile, you can `git clone` your app to your computer and start coding.
5. **IMPORTANT** : your first `git push` shall NOT be earlier than the first building ends

### Tips

* The first building lasts for 30 to 40 minutes, the progress can be seen on your app page (eg. https://foo-bar.rhcloud.com )
* By default, PHP 5.6.23 is choosen, which can be found in `misc/make.sh`
* The OpenShift `diy` cartridge documentation can be found at:
http://openshift.github.io/documentation/oo_cartridge_guide.html#diy
* To install new PHP Extensions just add them to `conf/php5/ext` and add `extensions={extensionname.so}` to `php.ini`



[PT-BR]
#PHP 5.6 + Driver do MongoDB + Apache

Esse *DIY cartridge* irá instalar o PHP 5.6.23 com o driver do MongoDB e irá lhe conceder permissão para alterar as configurações do Apache, que se encontram na pasta `conf`.

## Guia rápido

[![Clique para instalar Openshift](http://launch-shifter.rhcloud.com/launch/light/Click to install.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=diy-0.1&initial_git_url=https://github.com/LucasPadilha/openshift-php-apache.git&name=php)

1. Acesse https://openshift.redhat.com/app/console/application_type/cart!diy-0.1
2. Preencha **Source Code** com o seguinte: `https://github.com/LucasPadilha/openshift-php-apache.git`
3. Clique em **Create Application** e aguarde.
4. Após finalizar o carregamento, acesse o site da sua aplicação (ex.: foo-bar.rhcloud.com), clique em `start building` e deixe seu browser aberto. A página irá se atualizar automaticamente ao fim do processo, mostrando o `phpinfo`.
5. **IMPORTANTE**: Não dê `git push` para a aplicação antes de terminar o processo de construção.

### Dicas

* O processo de construção demora de 30 a 40 minutos.
* Você pode alterar a versão do PHP em `misc/make.sh`
* A documentação oficial do *DIY Cartridge* pode ser encontrada em http://openshift.github.io/documentation/oo_cartridge_guide.html#diy
* Para instalar extensões do PHP basta adicioná-las na pasta `conf/php5/ext/` e adicionar a linha `extensions={nomedomodulo.so}` no `php.ini`