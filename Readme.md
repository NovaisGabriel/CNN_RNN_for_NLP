<h1>CNN and RNN for NLP</h1>
<p align="justify">Este repositório visa criar um breve resumo e implementação de redes neurais recorrentes. É um repositório voltado mais para o estudo do autor, e portanto 
    não possui a pretenção de ser algo pronto, mas sim em permanente construção. O artigo fonte para este estudo e cujos textos e gráficos estão na apresentação disponibilizada neste repositório segue abaixo:
     </p>
<p align="justify"><a href="https://arxiv.org/pdf/1808.09772.pdf">https://arxiv.org/pdf/1808.09772.pdf</a></p>
<p align="justify">Um excelente link para um aprendizado mais robusto de RNN está em:</p>
<p align="justify"><a href="https://colah.github.io/posts/2015-08-Understanding-LSTMs/"> https://colah.github.io/posts/2015-08-Understanding-LSTMs/</a></p>
<p align="justify">Para exemplos de aplicação em NLP seguem os links abaixos:</p>
<p align="justify"><a href="https://colah.github.io/posts/2015-08-Understanding-LSTMs/"> https://colah.github.io/posts/2015-08-Understanding-LSTMs/</a></p>
<p align="justify"><a href="https://towardsdatascience.com/natural-language-processing-from-basics-to-using-rnn-and-lstm-ef6779e4ae66">https://towardsdatascience.com/natural-language-processing-from-basics-to-using-rnn-and-lstm-ef6779e4ae66</a></p>
<p align="justify">Agradecimentos aos autores que disponibilizaram publicamente o material de excelente qualidade nos links acima.</p>    
</p></p></p></p>
<h3>Dados</h3>
<p align="justify">Os dados utilizados para realizar a RNN simples no código disponibilizado encontra-se no link abaixo:</p>
<p align="justify"><a href="https://archive.ics.uci.edu/ml/datasets/Sentiment+Labelled+Sentences">https://archive.ics.uci.edu/ml/datasets/Sentiment+Labelled+Sentences</a></p>
<p align="justify">Conforme pedido  no site para realizar o download da base de dados seguem as referências: "<b>From Group to Individual Labels using Deep Features', Kotzias et. al,. KDD 2015"</b></p>
<h3>Sobre a RNN</h3>
<p align="justify">Trata-se de uma forma específica das redes neurais em que as camadas escondidas (Hidden Layers)
    comunicam-se entre si estabelecendo uma dimensão temporal, de maneira que a atualização tanto do feedfowrad quanto 
do backpropagation respeitam essa sequência da disposição interna da rede. Ela pode ser utilizada tanto para 
modelagem e previsão de séries temporais, como é utilizada em sua grande maioria, mas também pode ser
aplicada a outros estudos em que a disposição dos elementos dos dados possuem certa influência sobre a previsão ou estudo da própria modelagem. </p>

<h3> Problemas de aplicação</h3>

<p align="justify">Existem alguns problemas que podem surgir quando se faz o uso dessa técnica, prejudicando o processo de 
    aprendizado. Uma delas é o problema de Vanishing Gradient ou Exploding Gradient, que surge da retroalimentação das camadas 
    internas da rede, que pode ser longa, e assim a matriz de pesos quando possui valores pequenos, devido a multiplicação, pode
    ao final de uma época apresentar valores muito próximos a zero. O que equivalente pode ocorrer se a matriz possuir valores altos.
</p>
<p align="justify">Algumas soluções viáveis para contornar este problema podem ser implementadas, como truncar o procedimento do backpropagation, aplicar penalidades ou estabelecer limites máximos ou mínimos para 
    a matriz de pesos. Além disso existem ainda formas de inicializar a matriz de pesos de forma conveniente. Outra forma seria a aplicação das conhecidas Long Short-Term Memory Networks, ou então,
    LSTMs. Para estudos mais aprofundados do funcionamento das LSTMs sugere-se a leitura do material disponibilizado no link acima.
</p>
