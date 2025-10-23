# 🔐 Gerador de Senhas

Um simples **gerador de senhas** feito em **Python**, ideal para quem quer aprender sobre geração aleatória de strings e criação de senhas de forma rápida e prática.

---

## 📘 Sobre o Projeto

Este projeto gera uma senha de **8 caracteres aleatórios**, combinando letras, números e símbolos.  
É um exemplo simples, mas funcional, e pode ser facilmente adaptado para gerar senhas mais seguras ou maiores.

---

## 🚀 Como Usar

1. **Clone o repositório:**
   (git clone https://github.com/seu-usuario/gerador-de-senha.git)

2. **Acesse o diretório:**
   (cd gerador-de-senha)

3. **Execute o script:**
   (python gerador_senha.py)

4. **Resultado esperado:**
   (--------------------  
   a1!y2b#q  
   --------------------)

---

## ⚙️ Personalização

Você pode modificar o conjunto de caracteres ou o tamanho da senha conforme desejar.  
Basta editar o código e alterar a variável `caracteres` e o número de iterações no `range()`.

**Exemplo:**

(caracteres = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890!@#$%&*"  
tamanho = 12  # Defina o tamanho da senha aqui  

senha = ""  
for digito in range(tamanho):  
    aleatorio = random.choice(caracteres)  
    senha += aleatorio)

### 🔒 Dica de segurança:
Para gerar senhas mais seguras, substitua o módulo `random` por `secrets`:

(import secrets  
import string  

caracteres = string.ascii_letters + string.digits + "!@#$%&*"  
senha = ''.join(secrets.choice(caracteres) for _ in range(12))  
print(senha))

---

## ⚠️ Avisos de Segurança

- O módulo `random` **não é recomendado** para gerar senhas reais — use `secrets` para segurança criptográfica.  
- Evite armazenar senhas em **texto puro**.  
- Prefira senhas com **12 caracteres ou mais**.  
- Nunca compartilhe senhas publicamente ou em repositórios.

---

## 🧩 Requisitos

- Python **3.6+**  
- Nenhuma biblioteca externa é necessária.  

---

## 🛠️ Melhorias Futuras

- [ ] Permitir definir o tamanho da senha pelo usuário.  
- [ ] Adicionar suporte a argumentos via linha de comando.  
- [ ] Criar opção para gerar múltiplas senhas.  
- [ ] Adicionar uma interface gráfica (Tkinter).  
- [ ] Permitir exportar senhas para um arquivo `.txt`.  

---

## 🤝 Contribuindo

Contribuições são **muito bem-vindas!**  
Sinta-se à vontade para abrir **Issues** e enviar **Pull Requests** com melhorias, correções ou novas ideias.  

Se quiser melhorar a segurança, adicionar recursos ou criar uma interface, será um ótimo upgrade! 💪

---

## 📝 Licença

Este projeto está sob a licença **MIT** — você pode usar, modificar e distribuir livremente.  
Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

---

---

⭐ Se este projeto te ajudou, não esqueça de deixar uma **estrela** no repositório!
