## Modelagem de Dados sobre Futebol

Tabela Jogador:
	Nome: String
	Idade: Int
	Altura: Int
	Peso: Int
	Time: 1-1 Time

Tabela Time:
	Nome: String
	Divisão: Int
	Pais: String

Tabela Partida:
	Estadio: String
	Time_Casa: Time
	Time_Fora: Time
	Duração: Duration
	Gols_Casa: Int
	Gols_Fora: Int
	Posse_Casa: Float
	Posse_Fora: Float
	Cartões_Casa: Int
	Cartões_Fora: Int


Documento EventosPartida:
	Partida: Partida
	Gols: [{Tempo: Tempo, Jogador: Jogador, TimePontuador: Time}]
	Lances: [{Tempo: Tempo, JogadorFeitor: Jogador, JogadorRecebidor: Jogador, Lance: String}]
	Posse: [{Tempo: Tempo, Jogador: Jogador}]
