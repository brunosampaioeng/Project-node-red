# Project: Brokerage catalog and zip code search engine
## This project will display data collected from the BrazilAPI webpage in the following way:

### 1. Broken Catalog:
Provide a web page listing all the available brokers from the BrazilAPI
(https://brasilapi.com.br/docs#tag/Corretoras) in the following format:

```"${Name} - ${City} / ${CNPJ}"```

### 2. Zip Code Searcher
 Provide a web page capable to show details of a provided zip code using BrazilAPI
(https://brasilapi.com.br/docs#tag/CEP-V2).

### Option 1:
The zip code must be inserted as a route parameter.

### Option 2:
The zip code must be inserted in a input field.

## Note:
1- Extra points if you make both options for the question 2.
2- Extra points if you apply a good styling, doesn’t matter if you apply styles from a
framework/library or anything related.

### Prerequisites for viewing:
- [Node.js](https://nodejs.org/en/)
- [Node-RED](https://nodered.org/docs/getting-started/local)
- An active internet connection to access the [BrazilAPI](https://brasilapi.com.br/)

# Initialization:
### 1. Clone this repository:
```bash
https://github.com/brunosampaioeng/Project-node-red.git```

### 2. Navigate to the project directory:

```http://localhost:1880```

### 3. If you haven't installed Note-RED, follow the procedure below:

#### 3.1.  At the command prompt, enter the following code:
```npm install -g node-red```
#### 3.2. Start Node-RED:
```node-red```

### 4. Open Node-RED and access the dashboard through your browser using the following link:

```http://localhost:1880```

### 5. Importing the flow:
- Click on the menu in the upper right corner represented by the three-line icon;

- Click on "import";

- Paste the code or select the "flow.json" file from this repository;

- Click on deploy, next to the menu mentioned earlier.

## Use
### Access to the brokerage catalog:

```http://localhost:1880/brokers```

This page will contain a catalog of brokers from BrazilAPI following this logic:

```${Nome_Social} - ${Municipio} / ${CNPJ}```

### Acesse to the Zip Code Searcher:
```http://localhost:1880/zipcode/{cep}```

Replace {cep} with the actual zip code you want to search

#### The page will display data about the entered ZIP code following this logic:
- Street
- Neighborhood
- City
- State

### If the ZIP code is invalid, an error message will appear in a pop-up notifying you.

