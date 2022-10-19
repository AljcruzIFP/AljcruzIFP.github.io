![Image](images/CVavatar.png)

# Alejandro Cruz
## Curriculum Vitae



- **Teléfono: 666123456**
- **Población: Barcelona**
- **Email: ifp@formacion.es**



### Experiencia

1. Prácticas en NaIberia
   - 6 meses
     - Jornada completa
 
 <sub>Único encargado del departamento de IT en una de las empresas
 punteras de transporte y logística en Catalunya</sub>
 
 2. Técnico informático en NaIberia
    - Actualmente
      - Jornada parcial

<sup>Contratado en la empresa donde realicé las prácticas, único
encargado del departamento de IT</sup>

### Habilidades



### Estudios
Cursando grado medio en Sistemas Microinformáticos y Redes(SMX)
- [x] Primer año
- [ ] Segundo año
- [x] Prácticas

Cursos online en _Mastermind_[^1]
1. Python
2. Hacking Ético
3. Fundamentos Linux


###### Ejemplo de código propio:
```
#--Caesar Encrypt--
#Mayusculas y Minusculas
#Switch: 1 al 6
#https://www.asciitable.com/

def caesar_encrypt(text):
    result = ""
    for i in range(len(text)):
        char_position = ord(text[i])
        new_char_position = char_position + 6  #<--Switch para cambiar
        if new_char_position >= 97:
            new_char_position = new_char_position % 123
            if new_char_position <= 97:
                new_char_position = new_char_position + 97
        elif new_char_position <= 96:
            new_char_position = new_char_position % 91
            if new_char_position < 64:
                new_char_position = new_char_position + 65
        result = result + chr(new_char_position)
        print(result)
    return result


def caesar_decrypt(cipher_text):
    result = ""
    for i in range(len(cipher_text)):
        char_position = ord(cipher_text[i])
        new_char_position = char_position - 6  #<--Switch para cambiar
        if new_char_position <= 65:
            new_char_position = new_char_position + 26
        elif new_char_position >= 91 and new_char_position < 97:
            new_char_position = new_char_position + 26

        result = result + chr(new_char_position)
        print(result)
    return result


text = "SeCreToXxYyZz"
print(f"Plain Text: {text}")
cipher_text = caesar_encrypt(text)
print(f"Encrypted: {cipher_text}")
print(f"Decrypted: {caesar_decrypt(cipher_text)}")
 

```









[^1]: [Link a Mastermind](https://www.mastermind.ac/)
