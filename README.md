# 🔐 Gerador de Senhas

Um simples **gerador de senhas** feito em **Python**, ideal para quem quer aprender sobre geração aleatória de strings e criação de senhas de forma rápida e prática.

---

## 📘 Sobre o Projeto

Este projeto gera uma senha de **8 caracteres aleatórios**, combinando letras, números e símbolos.  
É um exemplo simples, mas funcional, e pode ser facilmente adaptado para gerar senhas mais seguras ou maiores.

---

🚀 Como Usar

Clone o repositório:

git clone https://github.com/seu-usuario/gerador-de-senha.git


Acesse o diretório:

cd gerador-de-senha


Execute o script:

python gerador_senha.py


Resultado esperado:

--------------------
a1!y2b#q
--------------------

⚙️ Personalização

Você pode modificar o conjunto de caracteres ou o tamanho da senha:

caracteres = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890!@#$%&*"
tamanho = 12  # Defina o tamanho da senha aqui


Também é possível substituir o módulo random por secrets para maior segurança:

import secrets
import string

caracteres = string.ascii_letters + string.digits + "!@#$%&*"
senha = ''.join(secrets.choice(caracteres) for _ in range(12))
print(senha)

⚠️ Avisos de Segurança

O módulo random não é seguro para geração de senhas reais (use secrets).

Evite armazenar senhas em texto puro.

Prefira senhas com 12 caracteres ou mais para aumentar a segurança.

🧩 Requisitos

Python 3.6+

Nenhuma biblioteca externa necessária.
