# Desafio 02 - Minhas Músicas

## 📝 Descrição
Projeto desenvolvido durante o curso de Java da Alura para praticar conceitos de **Orientação a Objetos**, incluindo:
- Herança
- Polimorfismo
- Encapsulamento
- Classes abstratas

## 🎯 Objetivo
Criar um sistema para classificar áudios (músicas e podcasts) com base em suas reproduções e curtidas, implementando a funcionalidade de adicionar favoritos.

## 🏗️ Estrutura do Projeto

### Classes principais:
- **Audio**: Classe base para todos os tipos de áudio
- **Musica**: Extende Audio, representa uma música com cantor, álbum e gênero
- **Podcast**: Extende Audio, representa um podcast com apresentador e descrição
- **MinhasPreferidas**: Classe para gerenciar e exibir áudios favoritos

## 💡 Conceitos aplicados

### Herança
```java
public class Musica extends Audio {
    // Musica herda atributos e métodos de Audio
}
```

### Polimorfismo
```java
public void inclui(Audio audio) {
    // Aceita tanto Musica quanto Podcast
    if (audio instanceof Musica) {
        Musica musica = (Musica) audio;
        // Lógica específica para música
    }
}
```

### Override
```java
@Override
public int getClassificacao() {
    if (this.getTotalDeReproducoes() >= 2000) {
        return 10;
    } else {
        return 7;
    }
}
```

## 🚀 Como executar
1. Compile o projeto
2. Execute a classe `Principal.java`
3. Veja a classificação dos áudios cadastrados

## 📚 Aprendizados
- Implementação de herança em Java
- Uso de polimorfismo para código mais flexível
- Verificação de tipos com `instanceof`
- Sobrescrita de métodos com `@Override`
- Organização de pacotes e classes

