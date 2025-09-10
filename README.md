# Projeto Terraform - Curso de Introdução

Este projeto contém exemplos e práticas do curso de introdução ao **Terraform**.

---

## 🚀 Pré-requisitos

- [Terraform](https://developer.hashicorp.com/terraform/downloads) instalado
- Git configurado
- (Opcional) Conta na AWS configurada via `aws configure`

---

## ▶️ Como executar o projeto

1. Inicialize o Terraform (baixa os providers necessários):
   ```bash
   terraform init

Visualize o plano de execução (o que será criado/modificado):

terraform plan


Aplique as mudanças:

terraform apply


Confirme com yes.

🗑️ Como destruir a infraestrutura

Para remover todos os recursos criados pelo projeto:

terraform destroy


Confirme com yes.

🧹 Como limpar caches locais do Terraform
1. Apagar cache local do projeto

Remove binários e metadados apenas desse projeto:

rm -rf .terraform
rm -rf .terraform.lock.hcl

2. Apagar cache global (⚠️ opcional)

Libera espaço em disco, mas na próxima execução o Terraform precisará baixar novamente todos os providers:

rm -rf ~/.terraform.d/plugins

📦 Boas práticas

Nunca versionar a pasta .terraform/ ou arquivos .tfstate

Sempre manter um .gitignore com as exclusões adequadas

Usar Remote State (S3, Terraform Cloud, etc.) em projetos reais

✍️ Autor: Edson Gomes do Rego