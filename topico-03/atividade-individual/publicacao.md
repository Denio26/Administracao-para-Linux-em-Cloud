# Publicação do site

## Nível escolhido

Nível 2 - Intermédio

## Rota escolhida

Nginx

## Ficheiros criados

* index.html
* sobre.html
* style.css

## Estrutura criada

```text
topico-03/
└── atividade-individual/
    ├── site/
    │   ├── index.html
    │   ├── sobre.html
    │   └── style.css
    ├── evidencias/
    ├── comandos.txt
    ├── publicacao.md
    ├── validacao.md
    └── README.md
```

## Local de publicação

Os ficheiros do site foram publicados no diretório:

```bash
/var/www/html/topico-03/
```

## Comandos principais utilizados

```bash
sudo apt update

sudo apt install nginx -y

sudo systemctl start nginx

sudo systemctl enable nginx

sudo mkdir -p /var/www/html/topico-03

sudo cp site/* /var/www/html/topico-03/

hostname -I

curl http://localhost/topico-03

cloudflared tunnel --url http://localhost
```

## Publicação HTTPS

Para disponibilizar o serviço publicamente na Internet foi utilizado o Cloudflare Tunnel.

Esta solução permitiu expor o serviço sem necessidade de configurar encaminhamento de portas (Port Forwarding) no router ou adquirir um domínio pago.

O Cloudflare forneceu automaticamente:

* URL pública;
* Certificado SSL/TLS;
* Ligação HTTPS segura.

### Comando utilizado

```bash
cloudflared tunnel --url http://localhost
```

### URL pública

```text
https://intro-usc-thread-nasa.trycloudflare.com/topico-03-individual/
```

## Resultado obtido

O site foi publicado com sucesso através do Nginx e ficou acessível tanto localmente como através de uma ligação HTTPS pública fornecida pelo Cloudflare Tunnel.

Foi possível navegar entre as páginas:

* index.html
* sobre.html

e verificar a aplicação correta do ficheiro CSS.

## Evidências

Consultar a pasta `evidencias/` para:

* Estrutura criada;
* Instalação e estado do Nginx;
* Publicação dos ficheiros;
* URL pública gerada pelo Cloudflare Tunnel;
* Acesso HTTPS ao site;
* Validação das páginas.

## Limitações encontradas

A URL pública fornecida pelo modo rápido do Cloudflare Tunnel é temporária e pode mudar sempre que o serviço é reiniciado.

Para um ambiente de produção seria recomendado utilizar um domínio próprio associado a um túnel permanente.
