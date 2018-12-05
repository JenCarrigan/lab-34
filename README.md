![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Project Name

### Author: Student/Group Name

### Links and Resources
* [sandbox](https://codesandbox.io/s/40w580184x)

### Modules
#### `index.js`
Entry point
Provides the store to all components

#### `store/index.js`
Creates the store and exports it with the reducers

#### `lib/api.js`
Uses superagent to fetch data from the server

#### `app.js`
Renders h2 and provides model to component RecordList

#### `list.js`
Class Records has methods componentDidMount which will call the api to get the most recent data from the server and put it into our store
Will render all the data from the store through state

#### `record.js`
Class Record has method componentDidMount which will grab the model's schema. Also has a method handlesubmit that will make a post request to the api.
Will render the form based on the schema

#### `actions.js`
Exports function get, which calls api and updates store with current data
Exports function post, which call api and updates store with posted data

#### `reducers.js`
Exports new or changed state based on get or post requests.

#### UML
![UML](https://raw.githubusercontent.com/JenCarrigan/data-structures-and-algorithms/master/%3Aassets/lab-34-UML.jpg)
