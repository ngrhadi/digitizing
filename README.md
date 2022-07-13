# Service For Digitizing Tools _(./service-tdb)_

This backend service Rest Full API can operate Read and Update data

## What going on in here ?

1. For dependency using <a href="https://node-postgres.com/" target="_blank">pg</a> and <a href="http://knexjs.org/" target="_blank">knex js</a>
2. Build on top of <a href="https://expressjs.com/" target="_blank">express js</a> as engine system for management routing in JavaScript
3. Total query on each file have 3 except buffer data it's just 2
4. 100% using JavaScript
5. Confiduring function has been return promise using async await
6. Has been testing using `postman`

## Where if wanna change query or primary define database ?

Go to folder data, for change database configuration, on folder queries to change some queries, and on controler folder for change some configuration some function

---

---

# Frontend for Digitizing Tools _(./rlayers)_

This is part create using `create react-app`, using context management for state and `react-query` as state-management for fetching, mutation and query data. Also using `react-router-dom `for routing mangement and configuring until `data-id`

## What's going on in here ?

1. Main library using <a href="https://openlayers.org/" target="_blank">openlayers</a> and `rlayers` as context component
2. All layer has been configuring using ref data from parent until child component
3. For each layer has own name as exactly same on backend
4. Ui library using `react-bootstrap`, and for form library using <a href="https://react-hook-form.com/" target="_blank">react-hook-form</a>

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
12. Upload data error from csv
13. Handle integrated data error with existing data
14. Display data error on map and table as requirement type data error

## When if we want change style layers ?

Please read <a href="https://mmomtchev.github.io/rlayers/api/#rfeature" target="_blank">this</a> if you wanna change some configuration styling, like color, zoom, extend map, etc.

---

---

# HOW TO SET UP THIS APP ?

1. Please create github account where can use in 2 setup type, after that all that's folder can be accessible
2. Install this list on your OS
   - <a>Node.JS</a>
   - <a>GIT</a>
   - <a>PostgreSQL with PostGIS (extension)</a>
3. After installation you can check in terminal using this command
   - `node -v` for showing your node version
   - `npm -v` for showing your npm version
   - after that you must install yarn as global `npm i -g yarn`
4. Setup your github on your pc, open `Git-Bash` and add your account
   - For guide and read more info please visit this <a href="https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup" target="_blank">link</a>
   - `git config --global user.name "YOU_USER_NAME"` dont backspace `"`
   - `git config --global user.email "YOUR_EMAIL"` dont backspace `"`
   - check this `git config --list` for show what your name and email in there.
   - if have been configured you can clone this repo
5. Clone repository
   - `git clone` _link_this_repo_
   - `cd digitizing`
   - `git clone --recurse-submodules` _link_rlayer_folder_repo_
   - `git clone --recurse-submodules` _link_service-tdb_folder_repo_
6. Installation package
   - Open terminal, go to digitizing folder
   - write `yarn`
   - after that `cd rlayers\ && yarn`
   - same as before `cd service-tdb\ && yarn`
   - check configuring with your local database in this file `service-tdb\data\index.js`
   - app ready to running
7. Running this app
   - go to directory `digitizing`
   - run `yarn dev`
   - your web browser will be show this app
   - please make sure to read on begin app
