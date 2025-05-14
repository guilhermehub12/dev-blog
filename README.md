# Layout Responsivo com Tailwind CSS

Este projeto utiliza o **Tailwind CSS** para criar um layout responsivo, ideal para apresentar uma lista de eventos, com um layout dividido entre uma coluna principal de posts e uma barra lateral de destaques e tópicos recomendados.

## Estrutura do Layout

O layout é composto por duas seções principais:
1. **Coluna Principal**: Exibe uma lista de posts com informações sobre eventos.
2. **Barra Lateral**: Exibe "Escolhas da Equipe" e "Tópicos Recomendados".

### Container Principal (`<main>`)
- **Classe**: `flex flex-col md:flex-row max-w-7xl mx-auto px-4 py-8 gap-8`
- O layout utiliza o **Flexbox** para organizar os elementos em colunas para telas pequenas e em linha (horizontal) para telas médias ou maiores.
- A largura máxima do conteúdo é definida com `max-w-7xl` e é centralizado horizontalmente com `mx-auto`.
- O espaçamento interno é ajustado com `px-4` (1rem) e `py-8` (2rem), enquanto `gap-8` define o espaçamento entre os itens filhos.

### Coluna Principal (`<section>`)
- **Classe**: `flex-1 space-y-8`
- A coluna principal ocupa o máximo de espaço disponível (`flex-1`) e possui espaçamento vertical entre os elementos com `space-y-8` (2rem).

### Posts
Cada post dentro da coluna principal é organizado com **Flexbox** e usa as classes:
- **Classe**: `flex flex-col md:flex-row justify-between border-b pb-6 gap-4`
  - `flex-col` para organizar os itens em coluna nas telas pequenas.
  - `md:flex-row` para dispor os itens em linha (horizontal) em telas médias ou maiores.
  - `justify-between` distribui o conteúdo com o maior espaçamento possível entre os itens.
  - `border-b` aplica uma borda na parte inferior, e `pb-6` dá um padding inferior de 1.5rem.
  - `gap-4` define o espaçamento entre os elementos filhos dentro de cada post.

### Imagens
- **Classe**: `w-full md:w-48 aspect-video flex-shrink-0`
  - A imagem ocupa 100% da largura disponível em telas pequenas e 12rem em telas médias (`md:w-48`).
  - `aspect-video` mantém a proporção de 16:9, garantindo que a imagem seja exibida corretamente.
  - `flex-shrink-0` impede que a imagem encolha se o espaço for reduzido.

### Barra Lateral (`<aside>`)
- **Classe**: `w-full md:w-72 space-y-8`
  - A barra lateral ocupa a largura total em telas pequenas e tem uma largura fixa de 18rem (`md:w-72`) em telas médias ou maiores.
  - `space-y-8` aplica espaçamento entre os itens dentro da barra lateral.

### Lista de Escolhas da Equipe e Tópicos Recomendados
- As listas utilizam `space-y-2` e `space-y-4` para definir espaçamento entre os itens.
- As tags de tópicos recomendados possuem classes como `bg-gray-100 px-3 py-1 rounded-full text-sm`, criando botões arredondados com fundo cinza claro e texto pequeno.

## Funcionalidades

- **Responsividade**: O layout se adapta automaticamente entre a visualização em coluna e em linha, dependendo do tamanho da tela.
- **Design Modular**: As seções são facilmente adaptáveis e podem ser personalizadas ou expandidas para novos conteúdos.
- **Estilo Limpo e Organizado**: O uso do Tailwind CSS permite um design claro e de fácil leitura, com espaçamentos consistentes e uma aparência moderna.

## Como Usar

1. Certifique-se de ter o **Tailwind CSS** instalado e configurado no seu projeto. Caso não tenha, consulte a [documentação oficial do Tailwind CSS](https://tailwindcss.com/docs/installation).
2. Copie o código HTML para o seu projeto.
3. Personalize os textos, imagens e links de acordo com a sua necessidade.
4. Se necessário, adicione mais posts ou seções para expandir o layout.

## Dependências

- [Tailwind CSS](https://tailwindcss.com/)

## Contribuindo

Se você deseja contribuir com melhorias para esse projeto, sinta-se à vontade para abrir um **Pull Request**.

```bash
git clone https://github.com/guilhermehub12/dev-blog.git


