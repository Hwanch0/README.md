# Finals Task 6: MongoDB Practice Task
## Task Description: 

### 1. Create a database
- Connect to a running mongo instance, use a database named `mongo_practice`.
 - use mongo_practice
   
![image](https://github.com/user-attachments/assets/cf6f8297-7500-4fe8-9db6-8c35195b3dee)


### 2. Insert data in the database
- Insert the following movies:
  -  Fight Club

   ![image](https://github.com/user-attachments/assets/feab9f0f-28fd-4a64-977c-8bd76ad3a018)

  -   Pulp Fiction
  
 ![image](https://github.com/user-attachments/assets/cc2482bd-70b9-45a0-9891-9d83e147b439)


  -  Inglorious Basterds

![image](https://github.com/user-attachments/assets/92da293a-8a7d-4a25-a733-97f32af82352)


  -  The Hobbit: An Unexpected Journey

  ![image](https://github.com/user-attachments/assets/1d84a218-d832-4043-b007-b945d5ae16ca)


  -  The Hobbit: The Desolation of Smaug

   ![image](https://github.com/user-attachments/assets/64cad6e6-1433-46bc-869a-4e10a458801b)


  -  The Hobbit: The Battle of the Five Armies

 ![image](https://github.com/user-attachments/assets/585713c5-b763-49c3-834a-4d0127c6447f)


  -  Pee Wee Herman's Big Adventure

  ![image](https://github.com/user-attachments/assets/815ad280-1083-4b91-adf9-17be51f5af4c)


  -  Avatar

 ![image](https://github.com/user-attachments/assets/47d5a392-cd24-4efc-9a3f-ea6e20492448)

 ### 3. Query data in the database
- Find all documents

  ## Query / Find Documents

- query the `movies` collection to

1. get all documents
```
db.movies.find()
```
![image](https://github.com/user-attachments/assets/650d4b8a-6ee4-4fec-8aa5-556db602abe2)

```
2. get all documents with `writer` set to "Quentin Tarantino"
```
db.movies.find({writer:"Quentin Tarantino"})
```
```
![image](https://github.com/user-attachments/assets/3733e11b-5339-407a-8001-2a1e55b4c360)
```
```
3. get all documents where `actors` include "Brad Pitt"
```
db.movies.find({actors:"Brad Pitt"})
```
![image](https://github.com/user-attachments/assets/b64a9c7b-b372-405a-b82e-c003bde90fd5)

4. get all documents with `franchise` set to "The Hobbit"
```
db.movies.find({franchise:"The Hobbit"})
```
![image](https://github.com/user-attachments/assets/c4093771-b19b-4e5a-8eae-bd1e68bc19ba)

5. get all movies released in the 90s
```
db.movies.find({year:{$gt:"1990", $lt:"2000"}})
```
![image](https://github.com/user-attachments/assets/d83a73d2-ec6c-45a1-ab7c-3a881c40327d)

6. get all movies released before the year 2000 or after 2010
```
db.movies.find({$or:[{year:{$gt:"2010"}},{year: {$lt:"2000"}}]})
```
![image](https://github.com/user-attachments/assets/fa451371-a1bd-4e8e-afe6-1b5ede363b9d)

### 4. Update data in the database
- Add synopsis to The Hobbit: An Unexpected Journey

![image](https://github.com/user-attachments/assets/a556d5e4-cd0f-4c5a-9305-fa5bf43f92bf)

- Add synopsis to The Hobbit: The Desolation of Smaug

 ![image](https://github.com/user-attachments/assets/19fbff26-4da6-41f0-a727-af1ec49b6fb9)


- Add actor "Samuel L. Jackson" to Pulp Fiction

   ![image](https://github.com/user-attachments/assets/14ee4d4b-7da2-47fa-8656-d76201f13df6)


### 5. Text search
- Find movies with "Bilbo" in synopsis

![image](https://github.com/user-attachments/assets/07a02825-4eee-4fa9-b61c-5a62410668f9)


- Find movies with "Gandalf"

![image](https://github.com/user-attachments/assets/b69261f3-b967-48f1-bcac-255a0fbee65d)


- Find movies with "Bilbo" but not "Gandalf"

![image](https://github.com/user-attachments/assets/f1cccbed-4f9e-4ae7-8d80-9661147e2e76)


- Find movies with "dwarves" or "hobbit"

  ![image](https://github.com/user-attachments/assets/5abf3990-ae77-4794-9034-3e9429429435)

- Find movies with "gold" and "dragon"

![image](https://github.com/user-attachments/assets/4047ef07-332b-4b4d-a159-6e89d06a8678)


### 6. Delete data in the database
- Delete "Pee Wee Herman's Big Adventure"

![image](https://github.com/user-attachments/assets/3862c882-58e4-44f8-b6a9-e47df6b37067)



- Delete "Avatar"

![image](https://github.com/user-attachments/assets/1ddd8be3-c76d-453d-8d14-ba64839181ac)

