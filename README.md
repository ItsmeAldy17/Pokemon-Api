# Pokemon-Api
Tugas Backend Development GDSC

## Prerequisites
- Node.js
- MySql

## Usage
- Domain: http://localhost:3000/api/
- Endpoint: http://localhost:3000/api/posts

## Setup
1. Clone this repository:

```
git clone https://github.com/yourusername/Pokemon-Api.git
```

2. Install the dependencies:

```
npm install
```

3. Create/set .env file:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=pokemon-api
```

4. Run the server:
```
nodemon npm start
```

5. Test the api with method:

- *Get* [show all data]: http://localhost:3000/api/posts
- *Post* [insert data]: http://localhost:3000/api/posts/store
- *Patch* [update data]: http://localhost:3000/api/posts/update/:id
- *Delete* [delete data]: http://localhost:3000/api/posts/delete/:id

**Example usage *Get* all data http://localhost:3000/api/posts:**
```
{
    "status": true,
    "message": "List Data Posts",
    "data": [
        {
            "id": 5,
            "nama": "Oddish",
            "deskripsi_pokemon": "Pokemon berbentuk jamur bunga bangkai",
            "elemen": "Racun"
        },
        {
            "id": 4,
            "nama": "Sandshrew",
            "deskripsi_pokemon": "Pokemon berbentuk trenggiling",
            "elemen": "Tanah"
        },
        {
            "id": 3,
            "nama": "Pikachu",
            "deskripsi_pokemon": "Pokemon berbentuk kelinci  listrik ",
            "elemen": "Listrik"
        },
        {
            "id": 2,
            "nama": "Squirtle",
            "deskripsi_pokemon": "Pokemon berbentuk kura-kura dengan canon air",
            "elemen": "Air"
        },
        {
            "id": 1,
            "nama": "Charizzad",
            "deskripsi_pokemon": "Pokemon berbentuk naga api",
            "elemen": "Api"
        }
    ]
}
```
**Example usage *Get* data by id http://localhost:3000/api/posts/1:**
```
{
    "status": true,
    "message": "Detail Data Post",
    "data": {
        "id": 1,
        "nama": "Charizzad",
        "deskripsi_pokemon": "Pokemon berbentuk naga api",
        "elemen": "Api"
    }
}
```

