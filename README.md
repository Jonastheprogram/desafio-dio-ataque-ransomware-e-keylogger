# Desafio-DIO-ataque-ransomware-e-keylogger
Este desafio consistia em simular um ransomware para fazer a criptografia de dados e também um keylogger furtivo e automático para a captura de teclas feitas no sistema.

# Criptografando Dados
No arquivo "Ransomware" possui um malware programado em python para simular um ataque ransomware utilizando a biblioteca de criptografia Fernet que consiste em 5 passos.

### 1. Gerar uma chave de criptografia e salvar
   
### 2. Carregar a chave gerada

### 3. Encontrar arquivos para criptografar

### 4. Criptografar os arquivos que estiverem na raiz do diretório

### 5. Mensagem de ameaça e engenharia social para o alvo

Quando o arquivo ransomware.py é executado ele pega os arquivos do diretório em que ele esta e faz a criptografia de todos eles, se tornando impossível fazer a leitura destes arquivos, só podendo ser feito a descriptografia se tiver a chave que foi gerada no momento em que foi feito a primeira criptografia. Esta simulação de malware mostra bem como é feita um ataque de ransomware, onde o crime acontece conforme o passo 5, o criminoso manda uma mensagem de ameaça para a vítima pedindo uma quantia boa de dinheiro, se essa pessoa não enviar a quantia para o criminoso não tera seus dados descriptografados(comando esse que só o atacante tem para ser feito a descriptografia), dados esses que podem ser muito importantes para o alvo podendo trazer vários tipos de prejuízos. *Mais detalhes sobre o comando no arquivo "ransomware.py"*


# Registro e monitoramento de digitos
O Keylogger é um malware que quando executado no sistema é monitorado e capturado em um arquivo de log todo evento de tecla digitado pelo usuário. No arquivo "keylogger_email.pyw" foi utilizado as bibliotecas pynput, smtplib e algumas outras para automatizar o processo de captura de logs para serem enviados no email desejado. O arquivo se mantem totalmente furtivo por ser um executável em pyw rodando em segundo plano a todo momento (mais detalhes no arquivo keylogger_email.pyw). Após o malware ser executado em uma máquina, tudo o que for digitado no sistema será enviado para o email do cibercriminoso como mostra a imagem:

<img width="533" height="325" alt="image" src="https://github.com/user-attachments/assets/101177a1-78ec-4b33-aa3c-76eb65e4c2be" />

Neste desafio o intuito é demonstrar como agem os atacantes, sempre nos lembrando como é extremamente importante adquirir sempre novas formas de se proteger contra ciberataques. 

### Como devemos nos proteger?
Podemos começar com antivirus e firewalls sempre atualizados, essa é uma parte básica e o mínimo para se defender de ataques, pois o atacante sempre esta em constante aprendizado. Cuidados com engenharia social, sempre utilizar ambientes para testes para controlar o isolamento de ameaças, como a Isadora Ferrão nos disse na aula "A nossa maior defesa não é o antivirús ou firewall é o nosso conhecimento" assim entendemos que é sempre importante entender, conhecer as novas ameaças, como elas agem e reagem, para assim podermos nos proteger melhor contra isso.

