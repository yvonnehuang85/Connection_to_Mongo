# Connection_to_Mongo
Check the id of docker container
>>docker ps -a 

>>docker exec -it [container_id] bash    
(docker exec -it 6d7f38e46555 bash)    

>>mongo

>>use admin

>>db.auth(“username”,”password”)
db.auth("root","123456")

>>database_name
(test)

>>db.createUser({user:”username”,pwd:"123456",roles:[{role:"dbOwner",db:”databaseName”}]})
db.createUser({user:"root1",pwd:"123456",roles:[{role:"dbOwner",db:"test"}]})

