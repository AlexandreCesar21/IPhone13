<h1>Projeto iPhone 13
</h1>

<p>Este projeto simula uma página de apresentação do iPhone 13, onde o usuário pode ver a imagem do dispositivo em várias cores e interagir com um círculo de fundo que muda conforme a cor do modelo selecionado. Ele utiliza HTML, CSS e JavaScript para criar uma interface dinâmica e responsiva.

</p>


<h2>Tecnologias Utilizadas
</h2>
<p>• HTML5</p>
<p>• CSS3</p>
<p>• JavaScript</p>

<h2>Estrutura do Projeto
</h2>
<h3>1. HTML</h3>
<p>O HTML cria a estrutura da página com os seguintes elementos principais:</p>
<p>• <b>Header:</b> Um menu de navegação com links para diferentes produtos da Apple e uma logo.</p>
<p>• <b>Main:</b> A seção principal onde a imagem do iPhone é exibida e as cores disponíveis para o produto são apresentadas. Também há um texto explicativo sobre o produto e o preço.</p>

<p>O código HTML inclui:</p>
<p>• Links para o estilo CSS e o favicon.
</p>
<p>• Imagens do iPhone e logo.
</p>
<p>• Um conjunto de botões de cor que alteram a imagem do iPhone e o fundo da página.
</p>


<h2>2. CSS</h2>
<p>O CSS é responsável pelo design e layout da página. Alguns dos principais detalhes são:</p>

<p><b>Reset de Estilos:</b> O uso de box-sizing: border-box e a remoção de margens e padding em todos os elementos para garantir consistência no layout.</p>
<p><b>Estilo do Header:</b> Um menu de navegação com uma cor de fundo escura (#1d1d1d), que destaca o link "iPhone" com um estilo de borda.</p>
<p><b>Estilo Principal:</b> A seção principal tem um layout de flexbox para alinhar a imagem e o texto de maneira responsiva. A imagem do iPhone é exibida em diferentes tamanhos de tela, e há um círculo de fundo que muda de cor conforme a seleção do usuário.</p>
<p><b>Botões e Interações:</b> Botões de cor que, ao serem clicados, alteram a imagem do iPhone e a cor de fundo da página.</p>


<p>Exemplos de estilo no CSS:</p>

```
.navigation ul li a:hover {
    color: #fff;
    border-bottom: 1px solid #fff;
}

.main-text .btn {
    padding: 10px 25px;
    background: #0071e3;
    border-radius: 20px;
    color: #fff;
    font-size: 1.5rem;
    transition: all 0.5s;
}

.main-img img {
    width: 200px;
    transform: rotate(-7deg);
}
```

<h2>3. JavaScript</h2>
<p>O JavaScript adiciona a funcionalidade interativa à página:</p>

<p><b>Função</b> <code>imgSlider</code>: Altera a imagem do iPhone conforme a cor selecionada.</p>
<p><b>Função</b> <code>circleChange</code>: Muda a cor do fundo circular, dependendo da cor do iPhone selecionado.</p>

<p>Exemplo de código JavaScript:</p>

```
/*Função de mudar o celular*/
function imgSlider(e){
    document.querySelector("#phone").src = e;
}
/*Função de mudar a cor do circulo*/
function circleChange(color) {
    const circle = document.querySelector(".circle")
    circle.style.background = color
}
```

<h2>4. Responsividade</h2>
<p>O layout é totalmente responsivo, adaptando-se a diferentes tamanhos de tela. A seção principal ajusta o conteúdo conforme a largura da tela, garantindo uma boa experiência de usuário tanto em dispositivos móveis quanto em desktops.</p>


