# Password_generator
<p>
The package Password_generator can be used to create strong and integral passwords.
 <p>
 <p>
import random, string<br/>
 <p>

<br/>
<p>
<p>
tamanho = int(input('Digite a quantidade de caracteres que sua senha deve conter:'))<br/>
<p>
chars = string.ascii_letters + string.digits + '!@#$%&*()-=+,.:;/?'<br/>
rnd = random.SystemRandom()<br/>
print(''.join(rnd.choice(chars) for i in range(tamanho)))<br/>
