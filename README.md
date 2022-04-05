# Password_generator
<p>
The package Password_generator can be used to create strong and integral passwords.
 <p>
 <p>
import random, string<br/>
from setuptools import setup, find_packages<br/>
 <p>
setup(<br/>
    name= 'Password-generator',<br/>
    version= '0.0.1',<br/>
    author= 'tomedev',<br/>
    author_email= 'sansion91@gmail.com',<br/>
    description= 'Password_Generator',<br/>
    packages=find_packages(),<br/>
)<br/>
<p>
<p>
tamanho = int(input('Digite a quantidade de caracteres que sua senha deve conter:'))<br/>
<p>
chars = string.ascii_letters + string.digits + '!@#$%&*()-=+,.:;/?'<br/>
rnd = random.SystemRandom()<br/>
print(''.join(rnd.choice(chars) for i in range(tamanho)))<br/>
