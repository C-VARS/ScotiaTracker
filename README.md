### Developed by C-VARS: 
### Callum Cassidy-Nolan, Vladimir Dyagilev, Alexander Yang, Raag Kashyap, Sophie Nam


### Overview
ScotiaTracker is the minimum viable product solution to a specific payment case between large supplier corporations small business owners. It implements the Request-to-pay functionality to allow for direct deposit transactions, eliminating the physical risk as well as friction caused by using cheques and cash. 

Placing emphasis on user experience and operational efficiency, ScotiaTracker is extensible to future applications of modern digital payment technology.

### Business Problem
Personas Involved:
- Small Business Owner (Customer)
- Supplier
- Driver

Friction Points:
- risk for drivers carrying physical payment (cheques, cash) 
- delay in processing checques or cash
- credibility risk
    - cheques bouncing
    - faulty products

### Our Solution

An Android app that allows Request-to-pay functionality.

ScotiaTracker closely aligns with the user interface of the official Scotiabank app - modern, and intuitive to use. It simplifies the user experience with the app by distinguishing the actions required for each persona, and prioritizing the most needed features for the users. By implementing the Request-to-Pay functionality, a solution to the proposed business problem, the operational efficieny is also greatly improved.

### Features

#### Driver
- Notify delivery 
- Notify arrival

#### Supplier 
- Observes the payment process

#### Customer
- Confirm Payment

#### All Users
- **Track** delivery
- View **invoice information** as well it's status (Pending, on the way, arrived, payment processed)
- The ability to **search through invoices** by id, the driver, supplier, or customer name
- **Sort invoices** by its status or date
- **Notification** and text system to alert relevant personas of the invoice's new status

## ScotiaTracker Mobile App
<p align="center">
  <img src="https://media.giphy.com/media/Y3vyP1gf5R6ESHasyW/giphy.gif">
</p>




#### Future Applications



##### Tech Stack Deep-Dive

###### Front-End
* Java
    * Design Patterns used:
        * Dependency Inversion: Interactions between MVP layers
        * Facade: Interactions with model were handled through a facade to simplify communcations
        * Strategy: Invoice sorting & searching strategies are plug & play (newest/oldest, by name etc... timsort & quicksort). Following Open/Closed principle.
* Retrofit

###### Backend
* REST api hosted on Heroku
* PostgreSQL
* [firebase information]
