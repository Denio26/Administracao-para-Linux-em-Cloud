# Tópico 1 - Preparação do Ambiente Linux

## Ambiente utilizado

**Trilho seguido:** Trilho A — VM Local

**Ambiente utilizado:**  
Máquina Virtual Linux executada localmente através do VirtualBox.

**Distribuição Linux utilizada:**  
Ubuntu Server 24.04 LTS

**Estado do ambiente:**  
Ambiente funcional, com acesso ao terminal e execução de comandos concluída com sucesso.

---

## Objetivo desta atividade

O objetivo desta atividade foi preparar um ambiente Linux funcional para utilização ao longo do módulo, garantindo acesso ao terminal, organização inicial do projeto e criação das primeiras evidências técnicas.

Esta preparação servirá de base para futuras atividades relacionadas com:

- administração Linux;
- segurança;
- serviços web;
- firewall;
- gestão de utilizadores;
- backups;
- monitorização.

---

## Estrutura criada

Foi criada a seguinte estrutura de diretórios e ficheiros:

```bash
linux-seguranca-cloud/
├── topico-01/
│   ├── evidencias/
│   ├── comandos-topico-01.txt
│   └── README.md
└── produto-final/
```

### Evidência da estrutura criada

<img width="564" height="116" alt="image" src="https://github.com/user-attachments/assets/ff5c3fa7-785b-4b78-b1ee-f06af90c2307" />
<img width="366" height="144" alt="image" src="https://github.com/user-attachments/assets/7903b684-93f1-4370-a52c-5626fe435c49" />


Exemplo de comando utilizado:

```bash
tree linux-seguranca-cloud
```

---

## Comandos executados

Durante a atividade foram executados vários comandos para identificação do ambiente Linux e organização inicial do projeto.

| Comando | Finalidade |
|---|---|
| `pwd` | Mostrar o diretório atual |
| `ls -la` | Listar ficheiros e permissões |
| `uname -a` | Identificar o kernel e sistema Linux |
| `hostnamectl` | Consultar informações do sistema |
| `mkdir -p` | Criar estrutura de diretórios |
| `touch` | Criar ficheiros vazios |
| `tree` | Visualizar estrutura de pastas |
| `whoami` | Identificar o utilizador atual |

### Evidência dos comandos

<img width="643" height="19" alt="image" src="https://github.com/user-attachments/assets/6d6b1454-fdd0-4e7e-8407-a94197a56815" />

<img width="508" height="20" alt="image" src="https://github.com/user-attachments/assets/67c741df-9379-4beb-a4d5-143d9e1d8d92" />

<img width="838" height="271" alt="image" src="https://github.com/user-attachments/assets/3eec84ae-8606-426d-9dc8-2ccd5229507c" />

<img width="665" height="173" alt="image" src="https://github.com/user-attachments/assets/199adf3f-a7ac-46b9-994c-dbd9d9aa3a57" />

---

## Conteúdo do ficheiro comandos-topico-01.txt

```txt
pwd -> mostra o diretório atual
ls -la -> lista ficheiros e permissões
uname -a -> mostra informações do kernel Linux
hostnamectl -> mostra detalhes do sistema
mkdir -p linux-seguranca-cloud/topico-01/evidencias -> cria estrutura de diretórios
touch README.md comandos-topico-01.txt -> cria ficheiros vazios
tree linux-seguranca-cloud -> apresenta estrutura do projeto
whoami -> mostra o utilizador atual
```

---

## Diferença entre VM, VPS e infraestrutura em nuvem

### VM (Máquina Virtual)

Uma VM é um sistema virtual criado dentro de um computador físico. Permite executar Linux num ambiente isolado, normalmente usando software como VirtualBox ou VMware.

### VPS (Virtual Private Server)

Uma VPS é um servidor virtual alojado num datacenter. O utilizador tem acesso remoto ao sistema e pode configurar serviços como se fosse um servidor dedicado.

### Infraestrutura em nuvem

A infraestrutura cloud utiliza recursos distribuídos e escaláveis disponibilizados por fornecedores como AWS, Azure ou Google Cloud. Permite criar servidores, redes e serviços sob procura.

### Linux no browser

É um ambiente Linux acessível diretamente através do navegador web, normalmente usado para aprendizagem, testes rápidos ou laboratórios online.

---

## Dificuldades encontradas

### Exemplo 1
Foram encontradas dificuldades iniciais na configuração da rede da máquina virtual.

### Exemplo 2
O comando `tree` não estava instalado por defeito e foi necessário instalar através do seguinte comando:

```bash
sudo apt install tree
```

---

## Próximos passos

Para o próximo tópico será necessário:

- garantir que o ambiente Linux permanece funcional;
- continuar a utilização do terminal Linux;
- aprofundar comandos de administração;
- preparar configuração de utilizadores e permissões;
- continuar a recolha de evidências técnicas.

---

# Evidências

## Screenshot do terminal ativo

<img width="564" height="116" alt="image" src="https://github.com/user-attachments/assets/ff5c3fa7-785b-4b78-b1ee-f06af90c2307" />

---

## Screenshot da estrutura criada

<img width="366" height="144" alt="image" src="https://github.com/user-attachments/assets/7903b684-93f1-4370-a52c-5626fe435c49" />

---

## Screenshot dos comandos executados

<img width="838" height="271" alt="image" src="https://github.com/user-attachments/assets/3eec84ae-8606-426d-9dc8-2ccd5229507c" />

<img width="370" height="163" alt="image" src="https://github.com/user-attachments/assets/9879f252-d4e0-4753-8e51-037f17ab5d2c" />

<img width="1191" height="620" alt="image" src="https://github.com/user-attachments/assets/91eb7bd1-5a95-479a-979b-e165bcef91c7" />

---

# Atividade Extra

## Ambiente de trabalho

### Tipo de ambiente

VM Local

### Sistema utilizado

Ubuntu Server 24.04 LTS

### Recursos disponíveis

| Recurso | Valor |
|---|---|
| CPU | 2 vCPU |
| RAM | 4 GB |
| Disco | 500 GB |

### Limitações

- Recursos limitados da máquina anfitriã
- Necessidade de gestão de espaço em disco
- Dependência do VirtualBox

### Observações

Esta estrutura será utilizada ao longo do módulo para organizar evidências, ficheiros de configuração, outputs de terminal e documentação técnica.

Pretende-se manter uma organização consistente para facilitar futuras entregas e revisão do trabalho realizado.

---

# Autor

**Nome:** Dénio Melo.  
**Curso/Módulo:** Linux, Segurança e Cloud  
**Data:** Maio 2026
