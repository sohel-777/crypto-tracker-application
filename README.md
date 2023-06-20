
# Crypto Tracker Application

CryptoTracker is the tracker you always needed. Compare different crypto currencies, look at their graphs - prices, total volumes, market cap, etc. Search from the top 100 Crypto currencies in real time and add them to your watchlist aswell.


## API Reference

#### Get all items

```http
  https://api.coingecko.com/api/v3/coins/markets?vs_currency=usd&order=market_cap_desc&per_page=100&page=1&sparkline=false&locale=en
```



#### Get item

```http
  https://api.coingecko.com/api/v3/coins/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |



## Color Reference

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| white | ![#fff](https://via.placeholder.com/10/fff?text=+) #fff |
| black | ![#111](https://via.placeholder.com/10/111?text=+) #111 |
| blue | ![#3a80e9](https://via.placeholder.com/10/3a80e9?text=+) #3a80e9 |
| grey | ![#888](https://via.placeholder.com/10/888?text=+) #888 |
|darkgrey | ![#1b1b1b](https://via.placeholder.com/10/1b1b1b?text=+) #1b1b1b |
| green | ![#61c96f](https://via.placeholder.com/10/61c96f?text=+) #61c96f |
| red | ![#f94141](https://via.placeholder.com/10/f94141?text=+)#f94141 |

## Deployment

Project Deployed Link 👇


  [Click here](https://crypto-tracking-application.netlify.app/)



## Features


#### Initial Setup - 


- Custom scroll Bar
- Custom selection.
- Disabling Image dragging + Folder Structure and code organisation.

#### Landing page - 

- Header - Mui Drawer.
- Text Stroke Hover animation - landing page.
- Framer Motion - The animation for phone and entrance animation for text.

#### Dashboard page - 

- Mui Tab component - for dashboard tabs (custom themed)

- ToLocaleString() - adds commas to numbers and ToFixed(2) - adds 2 decimal places
- Converting numbers to K,M,B - custom function
- Search functionality - accomplished using .filter()

- Pagination Mui - slicing the data in correspondence to the page number
- Wrote a js function to take us to the top of the page.

#### Coin page - 

- Used router params to get the id of the bitcoin

- Used react-chartjs-2 to make the graphs.
- Made a function to get the array of dates in x number of days.
- Used Mui Select to get the number of days, and had a function to get prices accordingly.
- Mui Toggle buttons for getting prices,mkt_cap,volume values.
- Used dangerouslySetInnerHTML attribute to render a string having html tags in it.
- Made a Loading component to make sure all the data was there, before rendering the components.
- Made a custom styled object to style Mui Components + Read More or Read Less functionality.


#### Compare Page - 

- For the 2 simultaneous graphs, we made 2 y-axis and 2 datasets.
- Select component mui, having the list of 100 coins.
- Also since comparison of the same coin makes no sense, we made sure that both selects have every coin other than the coin selected.

Light Mode Dark Mode - 

- Using local storage and data-theme variable in css
- Updating root variables according to the theme.

#### Watchlist- 
- localstorage - adding coins in an array
- localstorage - removing as well.
- useEffect -> watchlist page

#### Other features - 

- Using RWebShare npm package.

- Mui icons
- Seo + Code modularity and reusability.

- Gradient footer - gradient animation
- Added toasts - react-toastify for every action.
## Dependencies

Dependencies added 👇

```bash
   "@emotion/react": "^11.10.5",
    "@emotion/styled": "^11.10.5",
    "@mui/icons-material": "5.11.0",
    "@mui/lab": "^5.0.0-alpha.107",
    "@mui/material": "5.11.0",
    "@mui/styles": "5.11.0",
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "axios": "^1.2.1",
    "chart.js": "^4.1.0",
    "e": "^0.2.2",
    "framer-motion": "^7.6.19",
    "react": "^18.2.0",
    "react-chartjs-2": "^5.0.1",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.4.5",
    "react-scripts": "5.0.1",
    "react-toastify": "^9.1.1",
    "react-web-share": "^2.0.2",
    "web-vitals": "^2.1.4"
```
    
## Screenshots

#### Mobile  View 👇
![App Screenshot](https://i.ibb.co/ckcrVCw/Screenshot-2023-06-20-231650.png)

#### Landing Page Desktop  View 👇
![App Screenshot](https://i.ibb.co/Hq3NCpr/Screenshot-2023-06-20-231719.png)

#### Dashboard Page Grid View  👇
![App Screenshot](https://i.ibb.co/wyPWz94/Screenshot-2023-06-20-231744.png)

#### Dashboard Page List View 👇
![App Screenshot](https://i.ibb.co/dQLSbkz/Screenshot-2023-06-20-231814.png)

#### Dashboard Page Search Functionality 👇
![App Screenshot](https://i.ibb.co/W6sc29B/Screenshot-2023-06-20-231833.png)

#### Coin Page 👇
![App Screenshot](https://i.ibb.co/1KXY3vg/Screenshot-2023-06-20-231851.png)

#### Compare Page 👇
![App Screenshot](https://i.ibb.co/1JD27QD/Screenshot-2023-06-20-233057.png)
