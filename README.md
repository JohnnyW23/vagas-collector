# 👨‍💻 Vagas Collector 👩‍💻
Na busca por um estágio para alavancar minha carreira, tive a ideia de desenvolver o Vagas Collector! É um programa que coleta qualquer vaga dos sites Vagas e Indeed.
Assim que as vagas são coletadas, você escolhe se quer salvar uma planilha Excel ao fim do processo em um diretório de sua escolha. Tudo em passos simples!

## 🛠️ Ferramentas e tecnologias
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Tkinter](https://img.shields.io/badge/Tkinter-%23eeeeee?style=for-the-badge&logo=python&logoColor=%23222222)
![Selenium](https://img.shields.io/badge/Selenium-%23222?style=for-the-badge&logo=selenium&logoColor=%2343B02A)
![BeautifulSoup4](https://img.shields.io/badge/BeautifulSoup4-%23eee?style=for-the-badge&logo=python&logoColor=%23222222)
![JSON](https://img.shields.io/badge/JSON-%23dddddd?style=for-the-badge&logo=json&logoColor=%23000000)

### 📚 Principais bibliotecas Phyton utilizadas
🗂️ Tkinter\
🤖 Selenium\
🍛 BeautifulSoup4\
📊 OpenPyXL

Codificado em Python utilizando a biblioteca Tkinter para a criação da interface. Também houve a necessidade da linguagem tcl com o objetivo de implementar um tema
personalizado no Tkinter (tema este que não é de minha autoria, mas do usuário [rdbende](https://github.com/rdbende)).

## ⚙️ Requisitos
Para o programa funcionar corretamente no seu computador, você precisa ter instalado o Google Chrome, pois é a ferramenta usada pelo Selenium para buscar as ofertas.
Além disso, você precisa manter os seguintes elementos dentro da mesma pasta:
- pasta "forest-dark"
- Vagas Collector.exe
- forest-dark.tcl
- jobs.ico
- locais.json
- settings.json

Em outras palavras, mantenha a pasta "Vagas Collector" intocada.\
O executável está pronto para funcionar! Outros arquivos, como main.pyw e requirements.txt, servem justamente para fins de estudo e transparência sobre o código
usado no programa. Não são necessários para o funcionamento do executável, mas sinta-se à vontade para explorar, estudar e sugerir melhorias!

## 📖 Como o programa funciona
Primeiro, você vai se deparar com a interface simples e intuitiva do programa:

![Screenshot1](Vagas%20Collector%20screenshot%201.png)

- O campo do título da vaga é obrigatório por motivos óbvios.
- Estado e cidade não são obrigatórios, apesar de não fazer muito\
  sentido deixar em branco se você pretende procurar ofertas perto\
  da sua localização. Mas como é possível, então não há restrições\
  quanto a isso.
- O campo quantidade, que estabelece um número máximo de coleta de\
  vagas possíveis, também não é obrigatório. Mas se deixado em\
  branco, será considerado que você busca o máximo permitido, que\
  são 250 vagas.
- É obrigatório escolher no mínimo um dos portais, pois é onde será\
  feita a busca por ofertas. É possível escolher os dois juntos.

Assim que você tiver preenchido o formulário e iniciar o processo, basta aguardar o programa alertar o resultado. Caso você tenha escolhido os dois portais,
o programa começará a busca pelo site Vagas, e depois pelo Indeed.

![Screenshot2](Vagas%20Collector%20screenshot%202.png)

![Screenshot3](Vagas%20Collector%20screenshot%203.png)

Se a busca obteve 1 ou mais ofertas, você terá a opção de salvar uma planilha em Excel com as informações. Caso deseje, uma janela será aberta pedindo para você
escolher onde deseja que o arquivo seja salvo. Como cada site fornece categorias diferentes (por exemplo, apenas o Vagas disponibiliza o nível do cargo da
oferta, e apenas o Indeed disponibiliza o turno/tempo de trabalho), cada portal gerará sua própria planilha com o objetivo de manter a melhor organização
de suas informações coletadas.

![Screenshot4](Vagas%20Collector%20screenshot%204.png)

Agora você já pode conferir sua planilha criada com apenas 1 botão!

![Screenshot5](Planilha%20feita%20screenshot.png)

Perceba que é preciso formatar a tabela de maneira legível. Porém, você só precisa fazer isso na primeira vez que abrir seu arquivo. Caso você faça uma nova busca com o mesmo cargo
(escrito com os mesmos caracteres), o programa simplesmente irá carregar sua planilha, já formatada, e adicionará a nova informação! Provavelmente sua planilha terá
valores duplicados, mas basta redimensionar a tabela para ela cobrir todas as linhas e remover os valores duplicados nela.\
No caso de uma planilha do Indeed, é necessário mais cuidado pra remover os valores duplicados. Se você levar os links em consideração, nenhuma linha será
removida, pois os links das vagas no Indeed são dinâmicos e únicos. Portanto, para remover valores duplicados na tabela do Indeed, só é preciso desmarcar a caixa
da coluna "Links", ou leve em consideração apenas a coluna "Descrição", pois se toda vaga é única, nenhuma descrição se repetirá. E pronto!

## ⚠️ Observações

É possível que devido a constantes atualizações no arquivo HTML dos sites o programa fique obsoleto. Mas não se preocupe. Farei o possível para consertar e atualizar
o programa com as novas configurações necessárias. Mas se eu ainda não tiver feito isso e for do seu interesse, sinta-se à vontade para fazer uma pull request
com a solução!

## ❓ Dúvidas

Em caso de dúvidas, você pode entrar em contato comigo por aqui ou pelo meu [perfil no LinkedIn](https://www.linkedin.com/in/davinasc/).\
Muito obrigado e boa sorte na busca pela sua próxima vaga! 😉
