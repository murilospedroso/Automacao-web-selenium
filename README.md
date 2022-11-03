# Automacao-web-selenium

Com esse código será possível automatizar o processo de acessar uma url específica, iserir dados e acesso e clicar nas opções do site acessado.

Segue abaixo os passo feitos pelo código.

1 - Abrir o navegador (Neste caso o navegador será o Google Chrome).

2 - Acessar o site (neste caso será a página da hashtag Treinamentos).

3 - Clicar no botão "Login".

4 - Preencher os dados de e-mail e senha de acesso.

5 - Clicar no botão "Entrar".

6 - Acessar o Curso de SQL.

Observação: Esse código foi desenvolvido no Jupyter



########## Requisitos para execução do código #########

Instalar o Selenium

1 - Executar o Anaconda Prompt

2 - Digitar o comando "pip install selenium"


Instalar o Webdriver Manager

1 - Executar o Anaconda Prompt

2 - Digitar o comando "pip install webdriver-manager"




########## Detalhe sobre o Webdriver ##############

Para o Mozilla Firefox ==> Geckodriver
Para o Google Chrome ==> Chromedriver

Para manter o webdriver sempre atualizado utilizar as linhas abaixo no início do código

#servico = Service(ChromeDriverManager().install())
#navegador = webdriver.Chrome(service=servico)




########## Notas do desenvolvedor ###############

No comando "navegador.get" informe a url apenas com aspas simples no início e fim.

Exemplo: navegador.get('https://hashtag.eadplataforma.com/')

Para o comando "navegador.find_element", faça os passos abaixo.

1 - Clique com o botão direito na página à ser automatizada e selecione a opção "Inspecionar".

2 - Clique em cima de do item e copie o xpath dele.

3 - Lembre-se que para o método "send.key" você precisa inserir a informação correspondente.

Exemplo: navegador.find_element('xpath', '//*[@id="email"]').send_keys("murilo_pedroso@hotmail.com")

4 - Se o método for o "click", se trata de um botão, neste caso escreva da forma abaixo.

Exemplo: navegador.find_element('xpath', '//*[@id="btn_login"]').click()
