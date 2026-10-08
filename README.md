# Catálogo de Serviços

Aplicação web para organizar serviços de um pequeno negócio e montar um orçamento a partir do catálogo.

## Como usar

Abra `index.html` em um navegador atualizado. Não há instalação nem dependências externas.

1. Cadastre um serviço com nome, categoria e preço em reais.
2. Pesquise ou filtre o catálogo por categoria.
3. Adicione serviços ao orçamento e ajuste as quantidades.
4. Exporte o orçamento em JSON ou limpe os itens para começar outro.

Na primeira abertura, o catálogo apresenta três serviços fictícios de exemplo. Eles podem ser editados ou excluídos.

## Funcionalidades

- Cadastro, edição e exclusão de serviços.
- Pesquisa por nome e filtro por categoria.
- Orçamento com quantidades, subtotais e total.
- Preços calculados em centavos inteiros.
- Persistência local do catálogo e do orçamento.
- Exportação do orçamento em JSON com os valores vigentes no momento.
- Interface responsiva e mensagens acessíveis.

## Regras

O preço deve ser positivo, com até duas casas decimais e limite de R$ 1.000.000,00. A quantidade de cada serviço deve ser um inteiro entre 1 e 999. Alterar um serviço atualiza seu preço no orçamento aberto. Excluir um serviço também o remove do orçamento. O arquivo exportado mantém uma cópia dos preços e totais daquela exportação.

## Tecnologias e organização

HTML, CSS e JavaScript, reunidos em `index.html`. O catálogo armazena identificador, nome, categoria e preço em centavos. O orçamento referencia os serviços pelo identificador. Textos digitados são renderizados com `textContent`.

## Limitações

Esta é uma demonstração para estudo. Não há pagamento, emissão fiscal, envio a clientes, contas de usuário ou servidor. Os dados são locais e podem ser perdidos se o armazenamento do navegador for apagado. O arquivo exportado não pode ser importado nesta versão. Use apenas dados fictícios.

## Verificação manual

Cadastre um serviço de R$ 19,90, adicione três unidades e confira o subtotal de R$ 59,70. Teste edição, exclusão, pesquisa, filtro, quantidades inválidas e recarga da página. Confira o JSON exportado e navegue pela interface usando o teclado.

## Contexto

Projeto de estudo preparado com assistência de IA. Não representa experiência profissional.

## Validação realizada

Verificado em navegador local: cadastro, edição, exclusão, pesquisa e filtro, persistência, exportação JSON, rejeição de quantidade zero e atualização do orçamento ao editar ou excluir um serviço. Três unidades de R$ 19,90 totalizaram R$ 59,70. A página não apresentou rolagem horizontal em tela de 390 pixels nem erros de execução nesses cenários.
