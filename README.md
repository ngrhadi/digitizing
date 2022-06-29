# Service For Digitizing Tools (./service-tdb)

This backend service Rest Full API can operate Read and Update data

## What going on in here ?

1. For dependency using pg and knex js
2. Build on top of express js as engine system for management routing in JavaScript
3. Total query on each file have 3 except buffer data it's just 2
4. 100% using JavaScript
5. Confiduring function has been return promise using async await
6. Has been testing using postman

## Where if wanna change query or primary define database ?

Go to folder data, for change database configuration, on folder queries to change some queries, and on controler folder for change some configuration some function

---

# Frontend for Digitizing Tools (./rlayers)

This is part create using `create react-app`, using context management for state and `react-query` as state-management for fetching, mutation and query data. Also using `react-router-dom `for routing mangement and configuring until `data-id`

## What's going on in here ?

1. Main library using `openlayers` and `rlayers` as context component
2. All layer has been configuring using ref data from parent until child component
3. For each layer has own name as exactly same on backend
4. Ui library using `react-bootstrap`, and for form library using `react-hook-form`

## What's own feature on this app ?

1. Lock and unlock layers view
2. Show and hide layers view
3. Fetching on show layer view
4. Popup attribute data layer on hover
5. Snapping configure with range 10px
6. Controling tilelayers, controling scale, controling mini map view.
7. Table atribute for each layer except buffer data
8. Handle zoom layer id from Table
9. Handle edit atribute layer id from Table
10. Change geometry when draging on layers id
11. All have been route using react-router-dom

## When if we want change style layers ?

Please read <a href="https://mmomtchev.github.io/rlayers/api/#rfeature" >this</a> if you wanna change some configuration styling, like color, zoom, extend map, etc.
