# covid-graphql
A simple API that fetches the covid19-data for the countries that are avaliable.
The data curently include the dataset that provided https://coronavirus.jhu.edu/map.html 
and the data from NPHO.
(it's not the latest updated dataset).


This small project was inspired by and both datasets have been fetched form there,
https://github.com/Covid-19-Response-Greece/covid19-greece-api

# How to use.
 * Do docker-compose up, it should start intialize the library and start the application
 * Visit http://127.0.0.1:5000/graphql
 * Do for example :
     'query{
           getAllCountriesCovidInfo{
             country
             }
           }'

  It should return the list of countries for with we have data about the pandemic.
  
### Todo
- [x] Fetch data for single country by providing the name as input.

- [ ] Add mutations.

- [ ] Add NPHO (EODY) Greek covid19 data.

- [ ] Update data daily automaticaly.
