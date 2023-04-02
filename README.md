<div align="center">
    <img width="300" src="readme/logo.png" alt="Sportbay logo">
</div>
<br />
<div align="center">
    O Sportbay T uma expêriencia rápida e eficaz na compra de produtos da Sportbay, onde o usuário consegue pesquisar entre os grupos e categorias da loja os produtos que deseja comprar, e finalizar o pedido em menos de 1 minuto.
</div>
<br />
<div align="center">
  <kbd>
    <img width="250" height="450" src="readme/feature_home.png" alt="Image 1">
  </kbd>
  &emsp;
  <kbd>
    <img width="250" height="450" src="readme/feature_group.png" alt="Image 2">
  </kbd>
  &emsp;
  <kbd>
    <img width="250" height="450" src="readme/feature_products.png" alt="Image 3">
  </kbd>
</div>
<br />

## Tabela de conteúdo

* [Funcionalidades](#funcionalidades)
* [Técnicas e tecnologias utilizadas](#te-cnicas-e-tecnologias-utilizadas)
* [Estrutura de arquivos](#estrutura-de-arquivos)
* [Abrir e rodar](#abrir-e-rodar)
* [Licença](#licenc-a)

## Funcionalidades

* Departamentos

<img width="250" height="450" src="readme/feature_home.png" alt="Home">

<br />

* Tradução

<img width="250" height="100" src="readme/feature_language.png" alt="Language">

<br />

* Banner

<img width="250" height="450" src="readme/feature_banner.png" alt="Banner">

<br />

* Grupos

<img width="250" height="450" src="readme/feature_group.png" alt="Group">

<br />

* Categoria

<img width="250" height="450" src="readme/feature_category.png" alt="Category">

<br />

* Produtos

<img width="250" height="450" src="readme/feature_products.png" alt="Products">

<br />

* Carrinho de compras

<img width="250" height="450" src="readme/feature_cart.png" alt="Cart">

<br />

# Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas nas seguintes tarefas:

- [x] Departamento
- [x] Grupo
- [x] Categoria
- [x] Lista de produtos
- [x] Selecionar cores e tamanhos diferentes de produto
- [x] Adicionar ao carrinho
- [x] Buscar usuário
- [x] Buscar endereço
- [x] Buscar frete
- [x] Efetuar pagamento pix
- [x] Impressão do comprovante de pagamento
- [x] Traduções PT, ES e EN
- [ ] Efetuar pagamento via cartão de crédito

## Técnicas e tecnologias utilizadas

### Técnicas

- `componentização`: os componentes personalizados e compartilhados do projeto encontram-se na pasta "lib/src/widgets/"
- `componentização de telas`: os componentes especifícos de uma tela encontram-se na pasta da própria tela em "~/widgets/"
- `centralização de temas`: todas as cores e temas utilizados no app encontram-se na pasta "lib/shared/theme/app_theme".
- `centralização de fontes`: todas as imagens utilizadas no app encontram-se na pasta "lib/shared/assets/app_fonts".
- `centralização de icones`: todas as imagens utilizadas no app encontram-se na pasta "lib/shared/assets/app_icons".
- `centralização de imagens`: todas as imagens utilizadas no app encontram-se na pasta "lib/shared/assets/app_images".
- `centralização de máscaras`: na pasta "lib/utils/mask.dart" contém as informações de máscaras e formatação.
- `centralização de validações`: na pasta "lib/utils/validations/~" contém arquivos de validações de textos, como e-mail, telefone, CNPJ, CPF, etc.
- `multiplas linguagens`: o app possúi multiplas linguagens, seus arquivos de tradução estão localizados na pasta "lib/l10n".

### Tecnologias
-   [Intl 0.17.0](https://pub.dev/packages/intl) - Utilizada para gerar os arquivos de tradução
-   [Dio 4.0.6](https://pub.dev/packages/dio) - Utilizado para requests na API
-   [Provider 6.0.3](https://pub.dev/packages/provider) - Utilizado para MVVM como ViewModel
-   [Flutter native splash 2.0.1+1](https://pub.dev/packages/flutter_native_splash) - Utilizado para gerar uma splash screen nativa
-   [Carousel slider 4.1.1](https://pub.dev/packages/carousel_slider) - Utilizada para carrosel de imagens em detalhes do produto
-   [Auto size text 3.0.0](https://pub.dev/packages/auto_size_text) - Utilizada para que os textos se ajustem dinâmicamente
-   [Badges 2.0.3](https://pub.dev/packages/badges) - Utilizado para contagem de produtos no carrinho
-   [Fullscreen 1.0.3](https://pub.dev/packages/fullscreen) - Utilizado para esconder as bordas superiores e inferiores da tela
-   [Photo view 0.14.0](https://pub.dev/packages/photo_view) - Utilizado para visualizar imagens, dar zoom, scroll, etc.
-   [Connectivity plus 2.3.3](https://pub.dev/packages/connectivity_plus) - Utilizado para checar o estado da conexão da internet
-   [Flutter dotenv 5.0.2](https://pub.dev/packages/flutter_dotenv) - Utilizado para ler arquivos environment
-   [Permission handler 10.0.0](https://pub.dev/packages/permission_handler) - Utilizado para requisitar permissões do usuário
-   [Extended masked text 2.3.1](https://pub.dev/packages/extended_masked_text) - Utilizado para máscaras de texto
-   [Convert 3.0.2](https://pub.dev/packages/convert) - Utilizado para converter imagens para outros tipos
-   [Device info plus 4.0.0](https://pub.dev/packages/device_info_plus) - Utilizado para coletar informações do dispositivo
-   [Quick usb 0.4.0](https://pub.dev/packages/quick_usb/example) - Utilizado para fazer a conexão USB com dispositivos físicos
-   [Sentry flutter 6.6.1](https://pub.dev/packages/sentry_flutter) - Utilizado como Log Management
-   [QR flutter 4.0.0](https://pub.dev/packages/qr_flutter) - Utilizado para gerar QR codes
-   [Hex 0.2.0](https://pub.dev/packages/hex) - Utilizado pela impressora térmica
-   [Gbk_codec 0.4.0](https://pub.dev/packages/gbk_codec) - Utilizado pela impressora térmica
-   [Image 3.0.2](https://pub.dev/packages/image) - Utilizado pela impressora térmica

## Estrutura de arquivos

O acesso ao projeto está separado da seguinte forma:
```
lib/
├── l10n
    ├── all_locales.dart
    ├── app_en.arb
    ├── app_es.arb
    └── app_pt.arb
├── shared
    ├── assets/
    ├── theme/
    ├── widget/
    ├── cache_storage.dart
    └── constants.dart
├── utils
    ├── validations/
    ├── dialogs.dart
    └── mask.dart
├── src
    ├── model
        ├── api/
        ├── enum/
        ├── repository/
        ├── service/
        ├── product_model.dart
        ├── purchase_model.dart
        └── ...
    ├── view
        ├── product/
        ├── payment/
        └── ...
    └── view_model
        ├── product_provider.dart
        ├── department_provider.dart
        └── ...
├── route
└── main
```

Foi utilizado a arquitetura de projetos [MVVM](https://docs.microsoft.com/pt-br/windows/uwp/data-binding/data-binding-and-mvvra o desenvolvimento desse projeto.

## Abrir e rodar

**Para executar este projeto você precisa:**

- Ter o [Flutter 3.0.3](https://flutter.dev/docs/get-started/install) e o [Dart 2.17.5](https://dart.dev/get-dart) instalado na sua máquina;
- Ter alguma IDE como o [Android Studio 4.2](https://developer.android.com/studio);
- Clonar o projeto do [GitLab](https://gitlab.com/persys/pro-tork/sportbay-totem); 
- Ao abrir o projeto, execute o comando `flutter pub get` na raiz do projeto ou clique no arquivo [Pubspec.yaml](pubspec.yaml) e clique no botão no canto superior direito escrito `Pub get` e em seguida aguarde baixar as dependências do projeto;
- O processo de execução do aplicativo funcionará através de um botão de play na parte superior que ambas dispõem. Caso escolha rodar o projeto via linha de comandos, utilize o comando `flutter run`. Lembre-se de antes de executar o comando de navegar até a pasta do projeto antes.

## Licença

Esse projeto está sob licença de [Persys](https://persys.com.br/desenvolvimento/).

[Voltar ao topo](#tabela-de-conteu-do)<br>