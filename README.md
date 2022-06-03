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