_Created by Foxy 13.07.2021_
# Request Table
____
|   | GET | PUT| POST | DELETE|
|:----|:----------:|----------:|:----------:|:----------:|
| For one user | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| For all users | :white_check_mark: | :x: | :x: | :x: |
____
#Examples of requests
- GET
    - get all users. returns all users from database and http status.    
    http://localhost:8080/clients    
    - get user by id. returns user with __id=key__ from database and http status(requires id in address line)    
    http://localhost:8080/clients/id , id = userId of person you are going to get    
____
- PUT(update)
    - put user by id. (requires __id__ in address line and the whole body(__@RequestBody__))      
    :black_square_button: TODO with put request you can replace a single attribute, multiple attributes or the whole body(@RequestBody)    
    http://localhost:8080/clients    
    returns http status    
    
    :black_nib: example of body     
    {    
    "name" : "Foxy",    
    "email" : "mails@mail.ru",    
    "phone" : "8(900) 555-75-75"    
	}    
____
- POST(add new)
	- post user. (requires the whole body(__@RequestBody__))    
	with post request you can add new user to database    
    http://localhost:8080/clients    
    returns http status    
    
	:black_nib: example of body     
    {    
    "name" : "Foxy",    
    "email" : "maila@mail.ru",    
    "phone" : "8(900) 555-75-75"    
	}    
____
- DELETE
	- delete user by id. (requires __id__ in address line)    
	with delete request you can delete single user from database    
	_http://localhost:8080/clients/id_ , id = userId of person you are going to remove 
	