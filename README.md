# Counter

# Documentação do Primeiro App de Contador em Flutter

## Introdução

Este documento fornece uma documentação passo a passo para criar um aplicativo simples de contador usando o framework Flutter. O objetivo é ajudar iniciantes a entender os conceitos básicos do Flutter e criar um aplicativo funcional de contador.

## Pré-requisitos

Antes de começarmos, certifique-se de que você tenha instalado o Flutter e o Dart em seu sistema. Você pode seguir as instruções de instalação no site oficial do Flutter: [https://flutter.dev/docs/get-started/install](https://flutter.dev/docs/get-started/install).

## Passo 1: Configuração do Projeto

1. Crie um novo projeto Flutter usando o seguinte comando no terminal:

   ```
   flutter create contador_app
   ```

2. Acesse o diretório do projeto:

   ```
   cd contador_app
   ```

## Passo 2: Estrutura do Projeto

Dentro do diretório do projeto, você verá uma estrutura de diretórios como esta:

```
contador_app/
  ├── android/
  ├── ios/
  ├── lib/
  │    └── main.dart
  ├── test/
  ├── pubspec.yaml
  ├── README.md
```

- `lib/main.dart` é o ponto de entrada do aplicativo.

## Passo 3: Escrevendo o Código

Abra o arquivo `lib/main.dart` em seu editor de código e substitua o conteúdo pelo seguinte código:

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(ContadorApp());
}

class ContadorApp extends StatefulWidget {
  @override
  _ContadorAppState createState() => _ContadorAppState();
}

class _ContadorAppState extends State<ContadorApp> {
  int _contador = 0;

  void _incrementarContador() {
    setState(() {
      _contador++;
    });
  }

  void _decrementarContador() {
    setState(() {
      _contador--;
    });
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Contador Flutter'),
        ),
        body: Center(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: <Widget>[
              Text(
                'Contagem:',
                style: TextStyle(fontSize: 24),
              ),
              Text(
                '$_contador',
                style: TextStyle(fontSize: 48),
              ),
              SizedBox(height: 20),
              Row(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  ElevatedButton(
                    onPressed: _decrementarContador,
                    child: Icon(Icons.remove),
                  ),
                  SizedBox(width: 20),
                  ElevatedButton(
                    onPressed: _incrementarContador,
                    child: Icon(Icons.add),
                  ),
                ],
              ),
            ],
          ),
        ),
      ),
    );
  }
}
```

## Passo 4: Executando o Aplicativo

No terminal, navegue até o diretório do projeto e execute o aplicativo usando o seguinte comando:

```
flutter run
```

Isso iniciará o aplicativo de contador Flutter no seu dispositivo ou emulador.

## Conclusão

Parabéns! Você criou seu primeiro aplicativo Flutter de contador. Agora você tem uma compreensão básica de como criar uma interface de usuário simples e interativa com Flutter. Você pode estender este aplicativo e adicionar mais recursos conforme sua familiaridade com o Flutter aumenta. Continue explorando a documentação e tutoriais do Flutter para aprofundar seus conhecimentos.
