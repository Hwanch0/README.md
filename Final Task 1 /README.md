# Final  Task Lab 1: MySQL Basis

## ***Create an events table with fields***

- event_id (int, auto-increment, primary key)

- event_name (VARCHAR, up to 255 characters, not null)


![image](https://github.com/user-attachments/assets/cb1cdb54-0c41-4536-ae2a-8dc9aaad4735)


## ***Create an attendees table with fields***

- attendee_id (int, auto-increment, primary key)

- attendee_name (VARCHAR, up to 255 characters, not null)





## ***Create an event attendees table with fields***

- event_id (int, foreign key to events.event_id)

- attendee_id (int, foreign key to attendees.attendee_id)

- Composite primary key on (event_id, attendee_id)
  
![image](https://github.com/user-attachments/assets/dbce8a13-bb30-4924-b1d1-274e1e22fe24)




## ***Create an event sponsors table with fields***

- sponsor_id (int, auto-increment, primary key)

- event_id (int, foreign key to events.event_id)

- sponsor_name (VARCHAR, up to 255 characters, not null)

![image](https://github.com/user-attachments/assets/14aea1d1-e041-4e41-8e65-911b8eebdf3a)


 ## ***EER DIAGRAM***
![image](https://github.com/user-attachments/assets/5968f9fb-455d-43c1-86bf-fa21bc784e8b)

