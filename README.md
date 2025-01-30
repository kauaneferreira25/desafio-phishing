Etapas do Projeto:

1. Planejamento

Definição do Escopo:

Criação de uma página falsa para coleta de credenciais em um ambiente seguro.

Treinamento de um grupo sobre como reconhecer ataques de phishing.

Recursos Necessários:

Um computador com Kali Linux instalado.

Ferramenta Social-Engineer Toolkit (SET).

Servidor local para hospedagem do ataque (por exemplo, Apache).

Equipe participante para testes (com consentimento).

2. Configuração do Ambiente

2.1 Instalação e Atualização do Kali Linux

Certifique-se de que o Kali Linux esteja atualizado:

sudo apt update && sudo apt upgrade -y

Confirme que o SET está instalado:

sudo apt install set

2.2 Configuração do Servidor Local

Instale e inicie o Apache:

sudo apt install apache2
sudo service apache2 start

Verifique se o servidor está funcionando acessando http://localhost no navegador.

3. Criação do Cenário de Phishing

3.1 Usando o Social-Engineer Toolkit (SET)

Acesse o terminal como root:

sudo su

Inicie o SET:

setoolkit

Escolha a opção "Social-Engineering Attacks".

Selecione "Website Attack Vectors" e depois "Credential Harvester Attack Method".

Escolha "Site Cloner" para clonar um site autêntico.

Insira o URL do site a ser clonado (exemplo: http://www.instagram.com).

O SET gerará uma cópia da página e iniciará um servidor para hospedar o phishing.

3.2 Configuração de Redirecionamento Local

Obtenha o endereço IP da máquina com:

ifconfig

Acesse a página falsa através do IP gerado. Compartilhe o link apenas com participantes do teste em um ambiente controlado.

4. Execução do Teste

Informe os participantes que se trata de um treinamento.

Monitore como eles interagem com a página falsa.

Reforce a importância de verificar URLs, certificados SSL, e outros sinais de alerta.

5. Conscientização e Aprendizado

Apresente os resultados do teste para os participantes:

Quantos clicaram no link?

Quantos inseriram credenciais?

Discuta as técnicas de proteção:

Verificação de URLs.

Uso de autenticação de dois fatores (2FA).

Reconhecimento de sinais de phishing.# desafio-phishing


POSSIBLE USERNAME FIELD FOUND: email=amora.roxa@hotmail.com
POSSIBLE PASSWORD FIELD FOUND: pass=passwd

PARAM: prefill_contact_point=
PARAM: prefill_source=
PARAM: prefill_type=1
PARAM: first_prefill_source=
