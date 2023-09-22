# Counter

# Documentação do Primeiro App de Contador em Flutter - Configuração do Ambiente

Nesta documentação, iremos guiá-lo através da configuração do ambiente de desenvolvimento para criar um aplicativo de contador Flutter. Isso inclui a instalação do Android Studio e a configuração do Flutter nas variáveis de ambiente.

## Passo 1: Instalação do Android Studio

O Android Studio é uma IDE (Integrated Development Environment) popular para o desenvolvimento de aplicativos Android. Vamos começar instalando o Android Studio:

1. Faça o download do Android Studio em [https://developer.android.com/studio](https://developer.android.com/studio).

2. Execute o instalador baixado e siga as instruções para concluir a instalação.

3. Abra o Android Studio após a instalação e siga o assistente de configuração inicial para instalar os componentes necessários, como o Android SDK e as ferramentas do Flutter.

Passo 2: Instalando Flutter
 ```
git clone https://github.com/flutter/flutter.git -b stable
 ```

## Passo 3: Configuração das Variáveis de Ambiente

Agora que o Android Studio está instalado, precisamos configurar as variáveis de ambiente para que o Flutter possa ser acessado globalmente em seu sistema. Vamos realizar essa configuração no Windows.

### No Windows:

1. Abra o Painel de Controle do Windows.

2. Pesquise por "Variáveis de ambiente" na barra de pesquisa e clique em "Editar variáveis de ambiente do sistema".

3. Na seção "Variáveis de sistema", encontre a variável de ambiente chamada "Path" e clique em "Editar...".

4. Na janela "Editar Variável de Sistema", clique em "Novo" e adicione o caminho para a pasta "bin" do Flutter. O caminho padrão costuma ser `C:\src\flutter\bin`, mas pode variar dependendo de onde você instalou o Flutter.

5. Clique em "OK" para confirmar a adição do caminho do Flutter.

6. Para verificar se a configuração foi feita corretamente, abra um novo terminal e execute o seguinte comando:

   ```shell
   flutter doctor
   ```

   O Flutter Doctor irá verificar se todas as dependências estão instaladas corretamente. Se houver algum problema, siga as instruções fornecidas pelo Flutter Doctor para resolvê-lo.

Agora que o ambiente está configurado, você está pronto para criar seu aplicativo de contador Flutter como explicado na documentação anterior.

### No Linux e macOS:
Abra um terminal.

Navegue até o diretório raiz do seu usuário digitando o seguinte comando:

shell
```
cd ~
```
Abra o arquivo de perfil do seu shell, que pode ser ~/.bashrc, ~/.bash_profile, ou ~/.zshrc, dependendo do shell que você estiver usando. Use um editor de texto, como o nano, vim ou code, para editar o arquivo. Por exemplo, no Ubuntu, você pode usar o nano:

shell

```
nano ~/.bashrc
```
Ou, no macOS, você pode usar o nano também:

shell

```
nano ~/.bash_profile
```
Adicione as seguintes linhas ao final do arquivo para configurar as variáveis de ambiente para o Flutter:
shell
```
export PATH="$PATH:/caminho/para/o/diretorio/flutter/bin"
export PATH="$PATH:/caminho/para/o/diretorio/flutter/bin/cache/dart-sdk/bin"
```
Certifique-se de substituir /caminho/para/o/diretorio/flutter pelo caminho real onde o Flutter foi instalado em seu sistema.


Nota: No macOS, você pode precisar adicionar a seguinte linha também para configurar o caminho do Flutter:

shell
```
export PATH="$PATH:/caminho/para/o/diretorio/flutter/bin/cache/artifacts/engine/darwin-x64"
```
Salve as alterações no arquivo e saia do editor de texto.

Atualize as variáveis de ambiente executando o seguinte comando no terminal:

shell
```
source ~/.bashrc
```
Ou, no macOS:

shell
```
source ~/.bash_profile
```
Agora, as variáveis de ambiente para o Flutter devem estar configuradas corretamente em seu sistema Linux ou macOS. Para verificar se a configuração foi feita corretamente, abra um novo terminal e execute o seguinte comando:

shell
```
flutter doctor
```
O Flutter Doctor verificará se todas as dependências estão instaladas corretamente. Se houver algum problema, siga as instruções fornecidas pelo Flutter Doctor para resolvê-lo.

Com as variáveis de ambiente configuradas, você está pronto para desenvolver aplicativos Flutter em seu sistema Linux ou macOS. Certifique-se de ter o Android Studio (ou outra IDE) configurado e pronto para uso para o desenvolvimento de aplicativos Flutter.

Passo 4: Inicie o app no terminal onde o diretório onde fica localizado o download do app:
(De preferência dentro do disco C:)
 ```
flutter run - d Windows
 ```

## Conclusão

Agora você tem o ambiente de desenvolvimento configurado com o Android Studio e o Flutter devidamente configurado nas variáveis de ambiente. Você está pronto para criar seu primeiro aplicativo de contador em Flutter e explorar o emocionante mundo do desenvolvimento de aplicativos móveis com Flutter. Continue aprendendo e experimentando para aprimorar suas habilidades de desenvolvimento.
