# ALXprodev-Devops - Advanced Shell Scripting

This repository contains a series of shell scripts aimed at automating tasks related to the Pokémon API, processing and analyzing Pokémon data, handling errors, and utilizing parallel processing for speed improvement.

## Task Overview

### 0. API Request Automation
- **Objective**: Automate the process of making API requests to the Pokémon API and saving the results to a file.
- **Instructions**: 
  - Write a shell script to make a request to the Pokémon API (`https://pokeapi.co/api/v2/pokemon/`) for the Pokémon Pikachu.
  - Save the response in a `data.json` file.
  - If the request fails, log the error in `errors.txt`.
- **File**: `apiAutomation-0x00`

### 1. Extract Pokémon Data
- **Objective**: Extract specific data from the API response using advanced text manipulation tools like `jq`, `awk`, and `sed`.
- **Instructions**:
  - Write a script that extracts Pikachu's name, height, weight, and type from the `data.json` file.
  - Output the data in a human-readable format: "Pikachu is of type Electric, weighs 6kg, and is 0.4m tall."
- **File**: `data_extraction_automation-0x01`

### 2. Batch Pokémon Data Retrieval
- **Objective**: Automate the retrieval of data for multiple Pokémon and store it in separate files.
- **Instructions**:
  - Create a script that loops through a list of Pokémon (Bulbasaur, Ivysaur, Venusaur, Charmander, Charmeleon).
  - For each Pokémon, retrieve its data from the API and save it in a file named after the Pokémon (e.g., `pikachu.json`, `bulbasaur.json`).
  - Implement a delay between requests to handle potential rate-limiting issues.
- **File**: `batchProcessing-0x02`

### 3. Summarize Pokémon Data
- **Objective**: Create a report that summarizes the data for multiple Pokémon.
- **Instructions**:
  - Write a script to read the JSON files created in Task 2 and extract the name, height, and weight for each Pokémon.
  - Generate a CSV file containing the name, height, and weight of each Pokémon.
  - Use `awk` to calculate the average height and weight of the Pokémon in the report.
- **File**: `summaryData-0x03`

### 4. Error Handling and Retry Logic
- **Objective**: Implement error handling and retry logic for API requests.
- **Instructions**:
  - Modify the script from Task 2 to handle errors (e.g., network issues or invalid Pokémon names).
  - If a request fails, implement a retry mechanism that attempts the request up to 3 times before logging the error and moving to the next Pokémon.
- **File**: `batchProcessing-0x02`

### 5. Parallel Data Fetching
- **Objective**: Speed up data retrieval by using parallel processing.
- **Instructions**:
  - Write a script that fetches data for the Pokémon listed in Task 2 in parallel using background processes.
  - Ensure proper handling of background processes and wait for all processes to complete before continuing to the next step.
- **File**: `batchProcessing-0x04`

## Repository Structure
