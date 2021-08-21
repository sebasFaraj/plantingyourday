Setup
To set up and host the application yourself, first download the zip file. Here you’ll find all the files you need to start hosting the application. The first step is to go to your preferred IDE and make a new virtual environment within the project files. To get all the necessary installation simply execute pip install -r requirements.txt. Python should take care of the rest. Afterwards activate the virtual environment and use the flask run command in order to use the application. The file comes with some pictures and accounts to get started. Keep in mind that any information used will be stored on your computer. In the rare case of missing imports try to manually install the files yourself, perhaps they have been updated and require a newer version than the one found in requirements.txt. 

Database and Information
Navigating through the database, in the rare of case of errors and/or wanting to add more features, might be helpful in the usage of PlantingyourDay. There are 4 main tables, plants, owned,todo, and users in ascending importance. Plants is the simplest table, it holdsthe id, name, price, and brief description of the plant. The id is a primary key and the table is essentially just an inventory of all the available plants. It's used when checking a transaction and to display the available plants in the store. The owned table is a table keeps tracks of what users own which plants. It has a foreign key of owner which references the id column of users, a plant (plant name) column, a time column to store the users purchase time, and a stage column to keep track of a plants stage while growing. This feature has yet to be added so, if you're feeling inspired, I encourage anyone to do so with their own plants and growth rates. The next table is todo which has a Primary key of todo_id, a foreign key in owner that references id in the users table, a time_set and time_end table that store a varchar of the time the goal was set and when it ends, the goal itself, and the category of said goal. The home/index uses this table in order to display the goals of a user, it is edited anytime a goal is altered or completed. The last thing to note is the users table. It keeps track of the username, coins, account creation time, password hash, and historically completed goals of a user. Essentially everything works around this table, most user information is displayed through this table. Be weary when editing it as it can cause issues if columns are deleted or altered significantly. 



Video and Application Explanation
https://youtu.be/Lu8w3dUdUHg

Contact
If all else fails or you if you just have questions regarding the project and/or the link to the uploaded website, don't hesitate to contact me at sebasfaraj@gmail.com