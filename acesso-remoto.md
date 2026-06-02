# Acesso remoto por SSH

## Verificação do serviço SSH

Foi executado o comando:

```bash
systemctl status ssh
```

### Evidência

<img width="831" height="356" alt="image" src="https://github.com/user-attachments/assets/587cc6f3-f00f-4d95-8f9d-3f681a1cb67e" />

---

## Endereço IP identificado

Foi utilizado:

```bash
hostname -I
```

### Evidência

<img width="731" height="37" alt="image" src="https://github.com/user-attachments/assets/ba1827bf-017c-4445-8c1c-c2f7ee22e197" />


Endereço identificado:

```text
10.0.2.15
```

---

## Comando de ligação

```bash
ssh denio_melo@10.0.2.15
```

---

## Resultado obtido

Foi possível verificar que o serviço SSH está ativo e disponível para futuras ligações remotas.

---

## Limitações encontradas

O teste de ligação remota não foi realizado a partir de outro equipamento da rede, sendo apenas validada a disponibilidade local do serviço.
