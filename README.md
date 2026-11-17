# 🎬 Screenmatch (Spring Boot CLI)

Aplicação desenvolvida em **Java + Spring Boot** para consumo de API externa de filmes e séries, desserialização de JSON para objetos tipados e filtragem de temporadas e episódios via terminal.

---

## ⚙️ Tecnologias Utilizadas

- **Linguagem:** Java
- **Framework:** Spring Boot (sem módulo Web)
- **Build:** Maven (`mvnw`)

---

## 🏗️ Estrutura do Projeto

- `ScreenmatchApplication.java` — Ponto de entrada (`CommandLineRunner`)
- `principal/Principal.java` — Fluxo interativo de busca e manipulação de dados com Streams
- `service/ConsumoApi.java` — Cliente HTTP (`java.net.http.HttpClient`) para requisições à API externa
- `service/ConverteDados.java` & `IConverteDados.java` — Desserialização genérica de JSON com Jackson
- `model/` — Records/Entidades (`DadosSerie`, `DadosTemporada`, `DadosEpisodio`, `Episodio`)

---

## 🚀 Como Executar

```bash
# Clonar o repositório
git clone https://github.com/Salatielbg/Screenmatch-spring-sem-web.git
cd Screenmatch-spring-sem-web

# Executar com Maven Wrapper
./mvnw spring-boot:run
```

---

## 📫 Autor

**Salatiel Bonfim** · [LinkedIn](https://www.linkedin.com/in/salatiel-bonfim/) · [GitHub](https://github.com/Salatielbg)
