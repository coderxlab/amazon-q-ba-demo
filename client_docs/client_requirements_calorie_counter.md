# Client Requirements - Calorie Counter

## Project Overview
Getting and staying healthy requires a combination of mental balance, exercise, and nutrition. The goal of the Calorie Counter app is to help the user address nutritional needs by counting calories for various foods.

This app provides the number of calories based on the result of a user search for a type of food. The U.S. Department of Agriculture MyPyramid Food Raw Data will be searched to determine the calorie values.

## Technical Context
The app requires transforming raw data (MS Excel spreadsheet) into a JSON file format for easier loading and searching at runtime.

## User Stories

### Core Features

**1. Data Setup**
- ID: 96ee393d-85e7-45d9-93ee-df7c6a45f60e
- Status: incomplete
- Description: Developer will create a JSON file containing the food items to be searched. This will be loaded when the app is started.

**2. UI Panel**
- ID: 4c1fdc4c-f1e1-4de3-94e8-31a70774466a
- Status: incomplete
- Description: User can see a panel containing a food description input text box, a 'Search' button, and a 'Clear' button.

**3. Input Entry**
- ID: a5ebdaf5-df33-4f22-9f24-d12a5d20aa73
- Status: incomplete
- Description: User can enter search terms into the food description input text box.

**4. Search Function**
- ID: d1caa06c-d895-487d-a879-f2841fe13f9c
- Status: incomplete
- Description: User can click on the 'Search' button to search for the matching food.

**5. Input Validation**
- ID: de7954f2-9bac-4e22-ad06-3290d300beae
- Status: incomplete
- Description: User can see a warning message if no search terms were entered.

**6. No Results Handling**
- ID: 68f759c5-51fa-48cf-b9e8-216a3c343e0c
- Status: incomplete
- Description: User can see a warning message if no matches were found.

**7. Results Display**
- ID: c10b291c-e852-4ca0-82fd-e228845c1ad9
- Status: incomplete
- Description: User can see a list of the matching food items, portion sizes, and calories in a scrollable results panel that is limited to 25 entries.

**8. Clear Function**
- ID: cb007c08-f3bb-44ed-ba7e-9b5989b97b09
- Status: incomplete
- Description: User can click on the 'Clear' button to clear the search terms and results list.

### Bonus Features

**9. Results Count**
- ID: ff9341aa-a6e6-4250-b822-ab83cd3fc7db
- Status: incomplete
- Description: User can see the count of the number of matching food items adjacent to the results list.

**10. Wildcard Search**
- ID: 2cbc9020-2a70-4816-8578-d5108a00d6e8
- Status: incomplete
- Description: User can use a wildcard character in search terms.

**11. Pagination**
- ID: 1b1b9451-dca0-44c9-bde7-f8267f99c98a
- Status: incomplete
- Description: User can see more than 25 entries from a search by clicking a Down icon button to add more matching food items to the search results list.

**12. Performance Enhancement**
- ID: 2c1e6020-4b4c-49d9-9329-704e6190ea0a
- Status: incomplete
- Description: Developer will implement load the MyPyramid data into a database or a data structure other than an array for faster searching.

## Resources
- [MyPyramid Food Raw Data](https://catalog.data.gov/dataset/mypyramid-food-raw-data)
- [Example: Food Calculator](https://www.webmd.com/diet/healthtool-food-calorie-counter)

## Source
- **Confluence Page**: https://huyencp.atlassian.net/wiki/spaces/amazonqdem/pages/688129/Client+Requirements+-+Calorie+Counter
- **Space**: amazon-q-demo (amazonqdem)
- **Page ID**: 688129
- **Retrieved**: $(date)