CREATE TABLE scrittori (
    id_scrittore INT PRIMARY KEY,
    nome VARCHAR(50),
    cognome VARCHAR(50),
    nazionalita VARCHAR(50)
);

CREATE TABLE opere (
    id_opera INT PRIMARY KEY,
    titolo VARCHAR(100),
    data_uscita DATE,
    id_scrittore INT,
    FOREIGN KEY (id_scrittore) REFERENCES scrittori(id_scrittore)
);

CREATE TABLE teatri (
    id_teatro INT PRIMARY KEY,
    nome VARCHAR(100),
    citta VARCHAR(50),
    paese VARCHAR(50)
);

CREATE TABLE rappresentazioni (
    id_rappresentazione INT PRIMARY KEY,
    id_opera INT,
    id_teatro INT,
    data_rappresentazione DATE,
    FOREIGN KEY (id_opera) REFERENCES opere(id_opera),
    FOREIGN KEY (id_teatro) REFERENCES teatri(id_teatro)
);

ALTER TABLE rappresentazioni
ADD prezzo DECIMAL(6,2);
