Nome: Letícia Borges Campos
Módulo/Disciplina: UFCD 0154 - Estilos em CSS / UFCD 9963 - Edição Web
Formadora: Sara Monteiro

Descrição do Projeto 
Título: Redesign do Website da Aanifeira (Projeto Académico)
Este trabalho apresenta a reformulação (redesign) do website da associação Aanifeira (Associação de Proteção Animal). O objetivo principal foi reorganizar os conteúdos da associação, criar uma identidade visual mais apelativa e desenvolver uma experiência de navegação clara, funcional e responsiva para computador e telemóvel.

Website Publicado (GitHub Pages)
Link para o site online: https://leticia-borgescampos.github.io/projeto_aanifeira/

Conceito Visual

O conceito visual foi desenvolvido para transmitir confiança, afeto e clareza das informações institucionais, além disso, possui uma cor mais suave do que o website original e pemite ativar ou desativar o modo escuro
Paleta de Cores: Utilização de tons de verde suave como cor principal para transmitir ligação ao acolhimento de animais, combinado com fundos neutros e de maior contraste.
Tipografia: Leitura simples e estruturada, priorizando a legibilidade dos conteúdos em diferentes ecrãs. Utilização da fonte Playpen Sans para trazer um estilo amigável e que remete a escrita manual.
Layout: Disposição limpa dos blocos com Flexbox e CSS Grid, destacando os animais para adoção utilizando um carrossel de fotos e que facilita o acesso às informações.

Tecnologias Utilizadas

HTML5 Semântico: Estruturação com as tags
 <'header'> ;  <'nav'>; <'main'>; "<'section'>" ; <'article'> e <'footer'>
 
CSS3: Utilização de variáveis CSS 

(:root) ; Flexbox ; CSS Grid; media queries para responsividade e classes como :has() e :hover
Bootstrap: Utilizado como apoio à construção da estrutura do carrossel de adoção e setas de navegação e pop-up de confirmação de mensagem enviada.

Modos Diurno e Noturno

A mudança entre o modo claro e o modo escuro foi aplicado em CSS utilizando a classe :root:has(#modo-escuro:checked)
Modo Claro: Fundos claros (#f4f6f5), caixas a branco e texto em tom escuro para facilitar a leitura.
Modo Escuro: Fundos escuros (#111a14), cards em tom cinza-escuro (#1b261e) e texto claro para melhor contraste e não deixar o utilizador com a visão "cansada"
A mudança altera as variáveis globais de cor e é suavizada através de transições CSS.

Principais Variáveis CSS

No ficheiro style.css,  foram definidas variáveis no :root  para centralizar a paleta do projeto:
 --fundo-pagina: Define a cor principal do fundo da página
--superficie: Define a cor de fundo dos cards e caixas institucionais
--texto-principal: Muda a cor dos títulos e textos 
--cor-primaria: Define o tom verde principal do site
--cor-destaque: Utilizado na visualização de botões ao passar o rato (:hover)
--borda-cor: Define a cor de bordas e contornos

Transições CSS 

As transições CSS aplicados foram inseridas para dinamizar a experiência do utilizador:
Entrada de blocos (main > section):
Propriedades: opacity, transform
Duração: 0.6s
Temporizador: ease-out
Efeito: Os blocos são deslocados com um deslize suave e a opacidade aumenta quando a página é carregada
Alteração de Modos (Modo Escuro):
Propriedades: background-color, color, border-color
Duração: 0.4s
Temporizador: ease
Efeito: Transição suave das cores de todo o site ao ativar o check do botão do modo escuro

Botões e cards
(:hover):

Propriedades: background-color, transform

Duração: 0.3s

Função de temporização: ease

Efeito: Por exemplo, o botão de "Voltar ao topo" e os cards sobem um pouco (`translateY(-3px)) e mudam de cor para dar retorno claro de interatividade ao utilizador.

Fontes dos Recursos

Imagens: Fotos da associação e imagens dos animais retiradas dos meios de comunicação da Aanifeira
Webiste: https://www.pexels.com/pt-br/
Ícones e Emojis: Símbolos e emojis normais do sistema (como 📞 e ✉️) para identificar os contactos e botões

Dificuldades Encontradas e Soluções

1 - Alinhar o rodapé: 
Garantir que o paragrafo do rodapé e o botão "Voltar ao topo" ficassem alinhados na mesma linha sem desformatar no telemóvel ou computador

Solução: Apliquei o display: flex com justify-content: space-between e flex-wrap: wrap na classe .conteudo-rodape

2 - Formulário de contacto responsivo:
Inserir os 4 campos mantendo uma estrutura proporcional

Solução: Organizar o formulário dentro de uma caixa estilizada com Flexbox e usar o destaque com a classe :focus para tornar a visibildade mais acessível e indicar o campo ao utilizador.

3 - Ajuste do pop-up de mensagem:
Ajustar a mensagem pop-up e a imagem para se ajustarem à página e condizer com o estilo do site.

Solução: Utilizei o modelo de pop-up do bootstrap e ajustei a imagem usando as opções max-height ;  object-fit e  border-radius

4 - Ajuste de posicionamento das imagens, textos e cards:

Solução: Ajustei os tamanhos, margens e regras de posicionamento no CSS (utilizando larguras máximas, propriedades de alinhamento e as classes do Bootstrap), para garantir que o site ficasse visualmente harmonioso, limpo e responsivo.

5 – Posicionamento do carrossel considerando o formato mobile e desktop:
Manter o carrossel de forma que se adaptasse a diferentes tamanhos de ecrã, exibindo um cartão de cada vez no mobile para facilitar a leitura vertical, e dois cartões lado a lado por slide no computador para aproveitar melhor o espaço horizontal.

Solução: Utilizei classes do Bootstrap (d-none d-md-block) no HTML para mostrar um card por slide no telemóvel e dois no computador, combinada com Media Queries (@media (min-width: 992px)), Flexbox e limitação de largura máxima (max-width: 800px) no CSS, para garantir um bom alinhamento e imagens sem distorção com object-fit: cover.







Este é um projeto académico sem fins lucrativos e constitui um website não oficial desenvolvido para efeitos de avaliação na disciplina de  Estilos em CSS / Edição Web
