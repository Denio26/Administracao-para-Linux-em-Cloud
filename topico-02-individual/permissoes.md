# Permissões aplicadas

## Ambiente utilizado

VM local Ubuntu executada através do Oracle VirtualBox.

---

## Criação da estrutura de trabalho

Foi criada a estrutura solicitada para a atividade.

### Evidência

<img width="540" height="131" alt="image" src="https://github.com/user-attachments/assets/ab4885a2-112d-46d3-a745-326011d9979a" />

### Comandos utilizados

```bash
mkdir topico-02-individual
cd topico-02-individual
mkdir evidencias
touch comandos-utilizados.txt
touch permissoes.md
touch acesso-remoto.md
```

---

## Utilizador e grupos

Foram utilizados os seguintes comandos:

```bash
whoami
id
groups
```

### Evidência

<img width="668" height="116" alt="image" src="https://github.com/user-attachments/assets/2e5f92f9-936a-4a3a-bc84-80e75f6aa0fc" />

### Resumo

- whoami identifica o utilizador atual.
- id apresenta UID, GID e grupos.
- groups apresenta os grupos associados ao utilizador.

---

## Ficheiros criados

Foram criados os seguintes ficheiros:

```bash
mkdir teste-permissoes

touch publico.txt
touch restrito.txt
touch script.sh
```

### Evidência

<img width="662" height="115" alt="image" src="https://github.com/user-attachments/assets/d8cbc54a-670b-47cc-bd54-b4c3ec1a0864" />

<img width="668" height="83" alt="image" src="https://github.com/user-attachments/assets/d742064f-d409-4d76-8bad-12b5de3e95ff" />

---

## Permissões aplicadas

```bash
chmod 644 publico.txt
chmod 640 restrito.txt
chmod u+x script.sh
```

### Evidência

<img width="807" height="131" alt="image" src="https://github.com/user-attachments/assets/cb76f87e-6af2-4659-bec6-10aef2ce60ab" />


### Tabela de permissões

| Ficheiro | Permissão | Justificação |
|-----------|-----------|-------------|
| publico.txt | 644 | Permite leitura pública mas apenas escrita pelo proprietário. |
| restrito.txt | 640 | Restringe o acesso a utilizadores não autorizados. |
| script.sh | u+x | Permite execução apenas pelo proprietário. |

---

## Execução do script

Comando executado:

```bash
./script.sh
```

### Evidência

<img width="758" height="96" alt="image" src="https://github.com/user-attachments/assets/210d2343-44d9-4e34-bada-079d86fc3471" />

---

## Relação com o princípio do menor privilégio

O princípio do menor privilégio estabelece que cada utilizador deve possuir apenas as permissões estritamente necessárias para executar as suas funções. Desta forma reduz-se a superfície de ataque e evita-se a modificação indevida de ficheiros.
