# PokemonCapstoneProject![Pokeball](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/6f8b8ab7-8845-4dbf-af1c-7845b9523b95)

This is my Capstone Project for the Google Data Analytics Certification through Merit America. I chose to analyze previous Pokemon games.

# Ask

Introduction
This is my Capstone Project for the Google Data Analytics Certificate. For this I have chosen to do my own route. 
I am a junior data analyst at the Pokemon Company and I have been brought in to assist the creative team in finding inspiration for the next games by looking over the various creatures from previous games. 
The Pokemon Company is an international franchise that sells RPG (Role-Playing Games) video games and other products based on creatures from their games. In their video games, players catch, train, and battle creatures called ‘Pokemon’. A key feature of battling in the games is type match ups. Pokemon come in 18 different types, a pokemon can be either a single type or a dual type (two types). Depending on a Pokemon’s type they may be weak or strong against the other opponent’s Pokemon.

Key Stakeholders
Tsunekazu Ishihara, CEO of the Pokemon Company
Ken Sugimori, Character designer and art director of the entire franchise
The creatives teams from Pokemon, Game Freak, and Creatures creative teams

Business Task
Look over Pokemon type  and type combinations from previous games to find out how many Pokemon there are of each type. 

# Prepare

Data Sources:
Went to Kaggle and downloaded the Complete Pokemon Dataset (Gen I-IX). The dataset contains all 1010 Pokemon.
From Kaggle I also downloaded a video game sales dataset to compare the numbers of copies sold of the various Pokemon games throughout the years.
I also gathered information about money sales for the Pokemon games from a Pokemon website and entered the sales numbers into the sales dataset.
I uploaded the Pokemon dataset and video game sales dataset to google sheets. I prefer sheets over Excel because I find it much more user friendly. I first checked for duplicates and deleted them. To confirm the dataset’s reliability I compared the dataset to the official Pokedex online that contained information on every single Pokemon available. I manually entered all missing entries into the dataset, mostly some recent variants from newer games. There were also some misspelled entries that I corrected. I noticed there were two columns for type. While most Pokemon are two types this makes searching and filtering through the dataset harder for finding Pokemon based on type. I used the CONCATENATE function and merged the two columns into one and converted the type values to text. The Pokemon dataset was set, I had the rows organized by generation for easy comparison to see how the types had evolved over the years.
For the video game sales dataset, I filtered for Pokemon titled games only then copied and pasted those entries into another sheet. I created a column for revenue and entered the data from the Pokemon sales website. 
I stored all the files for the project onto my laptop in a folder labeled “Capstone Project”. In the folder I had another folder for the Pokemon dataset and another folder for the video game sales dataset. I also created separate folders for images and charts that I would create in Tableau.

# Process

Began by selecting the header row, clicked view, clicked freeze, clicked freeze row 1. This way as I’m scrolling I’ll be able to see the header row.
After experimenting with a few functions, I decided to use the COUNTIFS function because it allows me to search under more than one argument. In this case I needed to search Pokemon that were not only the same type but also belonged to the same generation.
Using the COUNTIFS function calculated how many Pokemon of each type and dual type in each generation.
Set up a second sheet for calculating pokemon types for each generation labeled “Pokemon_Types”.
Filtered through spreadsheets by single type, dual type, and generation.
Began work on the video game sales data by organizing it by revenue to see which games made the most money. Then organized by the number of copies sold.

# Analyze

After going over both datasets I found some interesting insights. 
The current generation of games, Pokemon Violet and Scarlet, have made the most money. However the first generation games(Pokemon Red, Blue, Green) have sold the most copies. The reason for this is most likely the Violet and Scarlet game sell for $60 for each copy while back in 1996 Pokemon Red and Pokemon Blue (Green existed only in Japan, Blue was made for North America) sold for $40 each. The other reason is probably because of the current state of the country’s economy. 
Pokemon types have also evolved over the years. For the first few generations there have been a lot of flying, water, and normal type Pokemon. Over the years they introduced new types: Dark and Steel in the generation 2 games(Silver and Gold) and then the Fairy type in generation 6(X and Y). After the third generation of games(Ruby and Sapphire) they added more Dark, Steel, Psychic, Ghost, and Dragon type Pokemon. The four most common types are: Water, Normal, Flying, and Grass. The four least common types are:  Ice, Steel, Ghost, and Fairy. To be fair the Fairy type is the newest type which is why there are so few Pokemon of that type. 
Also found that there are more dual type Pokemon than single type. For every type, except Normal type, there were more dual type Pokemon. Normal type was the only exception with 79 Pokemon that were only Normal type and 70 Normal dual type. Water was the closest to break even with 81 Water type and 88 dual Water type. Out of all the dual types Flying was the most common dual type with 126 Pokemon. Yet there are only 4 Pokemon that are pure Flying type and one of them is an alternate form of one of them. 

# Share
![PieChart_EachType](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/e79efe93-f483-4f34-9211-263833694ab3)
![Single and Dual Types](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/9438e9fe-c342-40a0-a1ea-e2e359b77256)
![Games_Years_Bar](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/ed14bff4-728d-4d16-888c-0f5ef783ed1d)
![Gen_1](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/7541bcb0-735c-4003-a6e7-136d9057eee1)
![Gen_2](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/83a8b118-1e1e-47f2-bdd1-c5200d67ccd9)
![Gen_3](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/f9b6bcc0-cb9a-4948-92d5-c2e72dfc22d8)
![Gen_4](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/561011a6-65ab-49f9-b0bf-87fedbf1f93d)
![Gen_5](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/56b7421e-86f3-4488-8036-9db24c5a4774)
![Gen_6](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/de28f81f-d92c-4845-8d69-1b1a74ab4bcc)
![Gen_7](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/430820b6-ce2d-4f44-992e-fe9e1745878d)
![Gen_8](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/f84b32da-529d-45fe-b485-95d0686fad94)
![Gen_9](https://github.com/DracaQueen/PokemonCapstoneProject/assets/112660805/0e6172c2-9884-44f2-bb7b-f0cb8e6a5ab2)


# Act

Based on the data I collected, for the next generation of Pokemon games it would be a good idea to create more Pokemon that are Fairy, Steel, Dragon, and Ghost type as well as new type combinations of those types. 
I also recommend having few or none Flying dual type Pokemon as there is more than enough, make more pure Flying type Pokemon.
When a player starts a new game often the first Pokemon they catch are Normal, Flying, Bug, and Water type. For the next generation of games mix it up by having Fairy, Dragon, Steel, and Ghost type Pokemon show up in the beginning rather than later in the game. This will definitely give a nice surprise especially to older fans of the games.
Another thing I would suggest is more Electric and Fighting type Pokemon to help balance the type match ups.
