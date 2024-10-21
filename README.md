# Mea-Kanu
Start of Plant Project

There are plant databases that exist but none yet with an api available to query from therefore im starting with this project to build some sort of api or project using the initial json data that has been compiled  

___
`meaKanu.json` is a file that consists of data parsed from Hawai'i County tax office species list PDF https://hawaiipropertytax.com/forms/Native%20Forest%20Dedication%20-%20Species%20List.pdf
___
## Structure
consists of an array of `Plant` which will generally be
```
String inoa, String description, String scientificName, String simpleInoa, Status status, ArrayList<Moisture> moisture
```
Where
* inoa: is its Hawaiian or common name
* scientificName: is its scientific name 
* simpleInoa: is its Hawaiian name without diacriticals such as okina or kahako for searchability
* status: is an enum consisting of the values `NATIVE`, `INTRODUCED`, `ALIEN`, `INVASIVE` representing its relation to Hawai'i
* moisture: is an array containing enum consisting of the values `DRY`, `MESIC`, `WET` representing the *Moisture Regime*

Possible future values
* elevation: numerical or general category
* habitat: possible overlap with elevation where values could be coastal, lowland, highland, alpine
* breaking NATIVE into Endemic or Indigenous
* uses
* photo
* Endangered species level (Protection status?)
___

Next:
* update simpleInoa
* Figure out project direction(s)
* API to query from (or just local if theres no reason for any business logic)
* UI for interactions
* AI project for identifying plants?
* ?