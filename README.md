# A MEME STREAM BACKEND
#### How to Use
1 - Extract the zip file memes.zip
2 - cd memes
3 - npm install (installs all the dependency)
4 - node src/index.js
5 - You are good to go A mongo atlas is used as the database instance for this project , so some old data is present

## Meme Schema
-- consists of Meme Provider Name ( userName) 
-- Meme Title ( content )
-- Meme Image URL ( image )
### Provides GET, POST and PUT endpoints
### Avaliable Endpoints
### Endpoint 1 : GET  (/memes)
Returns all available memes

### Endpoint 2 : GET (/memes/:id)
Returns the meme with the provided ID

### Endpoint 3 : POST (/memes)
Verifies the input data and adds the given meme to the database
Format of data in the POST request is : 
`{ "name" : "Providers Name" , "caption" : "Meme Caption " , "url" : "https://urltosomeimage.com/image.jpg" }`

### Enpoint 4 : PUT (/memes/:id)
Allows to edit the meme data except the Providers name

### Endpoint 5 : DELETE (/memes/:id)
Allows to remove or delete the meme of the provided id