<h1 align="center"><strong>Jquery</strong></h1>

<hr/>

<p align="center">
    <img src="/Images/jquery.png" alt="Jquery" title="jquery">
</p> 

# Seletores de elementos
    $ tag - $('h1')
    $ classe - $('.class')
    $ id - $('#id')

# Sequência de execução de código
    $ Espera o html e css carregar e depois executa a função - $(document).ready(function(){...})

# Selecionar atributos de tags
    $ Acessar src da imagem - $('img').attr('src')
    $ Atribuir novo valor ao atributo - $('img').attr('border', '5')

# Manipular conteúdo de elementos HTML
    $ Acessar conteúdo - $('#div1').html()
    $ Atribuir novo conteúdo - $('$div1').html('<p>Teste</p>')

# Recuperar e manipular valores de inputs (text) e selects
    $ Recuperar valor - $('nome').val()
    $ Atribuir novo valor - $('nome').val('Teste')

# Recuperar e manipular valor de check-box e radio
    $ Recuperar valor de input tipo radio - $('.sexo:checked').val()
    $ Recuperar valor de input tipo check-box :
        - $.each($('.interesse:checked'), (indice, valor) => {
            console.log(indice, valor.value);
        });

# Inserir e remover elementos HTML
    $ Inserir - $('ul').append('<li>Teste</li>') (prepend/after/before)
    $ Remover - $('ul').remove()

# Navegando entre elementos HTML
    $ .parent() - busca o elemento pai
    $ .closest() - procura por elementos pais
    $ .find() - procura por elementos filhos


# Manipulando CSS
    $('#topo').css({ 'color' : 'red' });
    $('#topo').css('color', 'red');

    .addClass('classe') - adiciona uma classe ao elemento selecionado

    .hasClass('classe') - verifica se um elemento possui determinada classe

    .removeClass('classe') - remove a classe de determinado elemento

# Eventos do navegador
    $(window).scroll(() => { }) - Scroll do mouse

    $(window).resize(() => { }) - Resize da página

# Eventos do mouse
    $('#btn1').mousedown(() => { }) - Evento ao passar o mouse sobre determinado elemento

    $('#btn1').click(() => { }) - Evento ao clicar em determinado elemento com o mouse

    $('#btn2').dblclick(() => { }) - Evento ao clicar duas vezes em determinado elemento com o mouse

    $('#div2').mousemove((e) => { }) - Evento ao mover o mouse sobre determinado elemento

    $('#divExterna').mouseenter(() => { }) - Evento ao entrar em determinado elemento com o mouse

    $('#divExterna').mouseleave(() => { }) - Evento ao sair de determinado elemento com o mouse

# Eventos do teclado 
    $('#teclado').keydown((e) => { }) - Evento ocorre ao clicar em determinado tecla do teclado

    $('#teclado').keyup((e) => { }) - Evento ocorre ao soltar determinada tecla

# Capturar valor de um campo
    $('#input').keydown((e) => { console.log($(e.target).val()); })

# Eventos de formulário
    $('#nome').focus((e) => { }) - Evento ocorre ao clicar em um input de formulário

    $('#nome').blur((e) => { }) - Evento ocorre ao desfocar de um input de formulário

    $('#opcao').change((e) => { }) - Evento ocorre ao alterar um valor de input type select

    $('form').submit((e) => { }) - Evento ocorre ao enviar um formulário

# Evitar comportamento padrão de determinado elemento HTML
    $('a').click(e => { e.preventDefault() }) - Evita redirecionamento da tag 'a'

# Adicionar eventos a tags filhas de determinado elemento HTML
    $('body').on('focus', 'input', e => { }) - adiciona evento 'focus' a todos os inputs filhos da tag 'body'

    $('body').off('focus', 'input', e => { }) - remove evento 'focus' de todos os inputs filhos da tag 'body'

    