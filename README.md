[![author](https://img.shields.io/badge/author-andersonsantana-red.svg)](https://www.linkedin.com/in/anderson-santana-53a51a69) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-365/) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/andersonandroid)

<p align="center">
  <img src="banner.png" >
</p>

# Ferramenta de busca de imagem de pornografia infentojuvenil
<sub>*Software Architec* da AI-HUB</sub>

O FAREJADOR é um software de código aberto portável que pode ser usado para buscar imagem de pornografia infantojuvenil, que muitos casos, o perito de informática se depara com situações que precisam analisar no local imagens que comprovem a materalidade da prisão em flagrante do individuo.

## Introdução:

Esse software é foi um trabalho de conclusão do curso da pôs-graduação em Computação Forense e Perícia Digital (instituição IPOG). Um software focado em desempenho e na eficacia na busca de imagem usando tecnologias modernas.

<p align="center">
  <img src="farejador.png?w=100">
</p>

**Tecnologias utilizadas:** Python, Hash, OpenCV, VP-Tree, SQLite.

**Características:**
* Suporte multiplataforma, testado em sistemas Windows e Linux
* Não precisa de instalação podendo ser executado em unidade removíveis
* Alto desempenho na indexação e na busca das imagens
* Relatório com as evidências encontradas com seus metadados
* Gera o hash das imagens encontradas para garantir a cadeia de custodia. 



## Setup:
Configuração do ambiente:


'''
def Consulta(**parametros):

	args = parametros
	tree = pickle.loads(open(args["tree"], "rb").read())
	hashes = pickle.loads(open(args["hashes"], "rb").read())
	image = cv2.imread(args["consulta"])	
	consultaHash = GeraHash(image)
	consultaHash = ConverteHash(consultaHash)
	inicial = time.time()
	results = tree.get_all_in_range(consultaHash, int(args["distance"]))
	results = sorted(results)
	final = time.time()
	tempo = format(final - inicial)
	
	if (len(results)) != 0:
		for (d, h) in results:
			
			resultPaths = hashes.get(h, [])
			for resultPath in resultPaths:
				
                resultPath
				
			resp = True

		return resultPath, d, tempo
	else:
		resultPaths = None
		d = None
		tempo = None
		return resultPaths, d, tempo
'''

* **Como usar o Histograma para Data Science:** https://bit.ly/2L2cMwy
* **Como Implementar Regressão Linear com Python:** https://bit.ly/2Li5pzY
* **Data Science: Investigando o naufrágio do Titanic:** https://bit.ly/2Ubr5SH
* **Como Tratar Dados Ausentes com Pandas:** https://bit.ly/31KWSMN
* **XGBoost: aprenda este algoritmo de Machine Learning em Python:** https://bit.ly/2UbRhws
* **Como criar uma Wordcloud em Python:** https://bit.ly/2OxsphM
* **Como lidar com dados desbalanceados:** https://bit.ly/2ZlaNsV
