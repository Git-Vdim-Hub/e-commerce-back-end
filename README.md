# e-commerce-back-end
## Description

- Internet retail, also known as **e-commerce**, is the largest sector of the electronics industry, generating an estimated $29 trillion in 2019. E-commerce platforms like Shopify and WooCommerce provide a suite of services to businesses of all sizes. 

- Due to e-commerce prevalence, understanding the fundamental architecture of these platforms is imparative as a full-stack web developer.

- Providing an e-commerce back-end solution to a buisness is a pivotal step for taking a buisness into the web sphere. 

- During this project I leared how to integrate SQL with expressjs using javascript with the npm package sequelize. After developing table models with sequelize I used them to route API requests with expressjs.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

After cloning repo, please make sure you have nodejs installed then run the following command:
```
npm i
```
After installation add a .env file in the root of the file system and add the following variables with your own credentials:
DB_USER = root
DB_NAME = ecommerce_db
DB_PASSWORD =
Make sure you have sql installed. If you do not please follow [sql install guide](https://coding-boot-camp.github.io/full-stack/mysql/mysql-installation-guide)

Once SQL is installed, cd into the db folder, log into sql and run the following command:
```
SOURCE schema.sql
```
After quit out of sql, cd back into the project root directory and run the following command:
```
npm run seed
```

Additionally, please install [insomnia](https://insomnia.rest/download) to test out the API calls with the application 
## Usage
Once everything is set up, run the following command to get started:
```
npm run start
```
or
```
npm run swatch
```
to use nodemon

Inside insomnia web app, run the following possible commands for the GET, POST, PUT and DELETE requests:
* GET:
- //localhost:3001/api/products
- //localhost:3001/api/tags
- //localhost:3001/api/categories
- //localhost:3001/api/products/1
- //localhost:3001/api/tags/2
- //localhost:3001/api/categories/3

* POST:
- //localhost:3001/api/products/
- {
   "product_name": "Basketball",
   "price": 200.00,
   "stock": 3,
   "tagIds": [1, 2, 3, 4]
}
-  //localhost:3001/api/categories/
- {
   "category_name": "Underwear"
}
-  //localhost:3001/api/tags/
- {
   "tag_name": "Cool Tag"
}

* PUT:
-  //localhost:3001/api/products/6
- {
   "product_name": "NBA Official Basketball",
   "price": 200.00,
   "stock": 3,
   "tagIds": [1, 2, 3, 4]
}
- //localhost:3001/api/categories/6
- {
   "category_name": "Undergarments"
}
-  //localhost:3001/api/tags/9
- {
   "tag_name": "Super Cool"
}

* DELETE:
-  //localhost:3001/api/products/1
-  //localhost:3001/api/categories/1
-  //localhost:3001/api/tags/3

Instructions and examples for use including screenshots and github repo/page.

- Click link to view repo: [Github Repo](https://github.com/Git-Vdim-Hub/e-commerce-back-end)
- Walk through [video](https://drive.google.com/file/d/1zQB6yQrS03AALlCwt6CcEaWlG2bB8YjU/view)
## Credits

This application was built with the use of [nodejs](https://nodejs.dev/en/) and the following npm dependencies: 
[sequelize](https://www.npmjs.com/package/sequelize?activeTab=readme), 
[dotenv](https://www.npmjs.com/package/dotenv), 
[nodemon](https://www.npmjs.com/package/nodemon), 
[mysql2](https://www.npmjs.com/package/mysql2),
[express](https://www.npmjs.com/package/express)
## License

[MIT](https://choosealicense.com/)
