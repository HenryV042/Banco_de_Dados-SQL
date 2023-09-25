# Banco_de_Dados-SQL


## 1. Selecione todos os dados dos países da tabela_paises;
```SQL
SELECT * FROM tabela_paises;
```
## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/6d6e17e7-b168-4543-904b-44c08a690e88)

## 2. Selecione todas as cidades cujo país seja brazil;
```SQL
SELECT * FROM tabela_paises WHERE pais = 'Brazil';
```
## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/29bfcc2f-4122-4711-818b-b30e73cd9a72)

SELECT * FROM table_cidades WHERE pais = 'Brazil';
## 3. Selecione todas as cidades cuja região(estado) é ceará;
```SQL
SELECT * FROM tabela_paises WHERE regiao = 'Ceará';
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/6c7dce56-7cdb-427b-ba53-4ad54d72d0aa)

## 4. Utilize a função count para saber quantas regiões(estados) existem na China, utilize também o group by;
```SQL
SELECT COUNT(regiao) FROM table_cidades WHERE pais = 'China' GROUP BY pais;
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/b19fc20f-1711-47a3-ba5c-f8da0a6c4e9c)

## 5. Quais regiões, diferentes, existem no Canadá?
```SQL
SELECT DISTINCT regiao FROM tabela_paises WHERE pais = 'Canada';
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/abe5f3a0-396f-4539-92f0-27e78732b51b)


## 6. Quantos países diferentes existem na tabela 'tabela_paises';
```SQL
SELECT COUNT(DISTINCT pais) FROM tabela_paises;
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/49cf5303-047e-4097-90a5-10a780109faa)

## 7. Quantas cidades diferentes existem no brazil;
```SQL
SELECT COUNT(DISTINCT cidade) FROM tabela_paises WHERE pais = 'Brazil';
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/45678dde-35b8-467d-91d5-3a9c35fd662a)

## 8. Selecione os países e quantas regiões cada país possui;
```SQL
SELECT pais, COUNT(DISTINCT regiao) FROM tabela_paises GROUP BY pais;
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/e26bf9f8-ad45-4259-a935-0e59368164c3)

## 9. Quantas pessoas com nome começando em 'João' existem no banco?
```SQL
SELECT COUNT(*) FROM tabela_paises WHERE nome LIKE 'João%';
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/229f974d-1044-476e-a288-fdf1e7beab72)

## 10. Quantas pessoas têm o nome John?
```SQL
SELECT COUNT(*) FROM tabela_paises WHERE nome = 'John';
```
## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/4cbae27a-8a3c-46f5-9ffd-77a761b98942)

## 11. Ordene os nomes dos países sem repetição em ordem alfabética;
```SQL
SELECT DISTINCT pais FROM tabela_paises ORDER BY pais;
```

## Saída:
![image](https://github.com/HenryV042/Banco_de_Dados-SQL/assets/111819715/843fc167-f3a0-4df9-b168-54ea5e4a8b3d)


