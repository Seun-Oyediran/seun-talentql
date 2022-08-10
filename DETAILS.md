# How does this work

## Steps in creating the app

- On load of the app. It fetches the first set of data and stores the result in a global variable with the page set to 1
- It then replaces the table rows with the new data that has just been fetched.
- When the next button is clicked, if the current page is an odd number, it will index the previous data stored globally and get the next page else it fetches another set page of data with page N + 2. i.e 1, 3, 5.
- When the prev button is clicked, if the current page is an even number, it will index the previous data stored globally and get the previous page else it fetches another set page of data with page N - 2. i.e 5, 3, 1
- During data fetching both buttons are disabled to prevent indexing data has not been fetched
- There is loader that shows when fetching data and it shows the current page when it has finished fetching data.
