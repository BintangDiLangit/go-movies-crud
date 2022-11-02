# Go Movies CRUD

Build with Go 1.19.3

## Installation

Run Locally

```bash
  git clone https://github.com/BintangDiLangit/go-movies-crud.git
  cd go-movies-crud
  go build
  go main.go
```

Open at browser (firefox, google chrome, etc)

```bash
  http://127.0.0.1:8080
```

## API Reference

#### Get all movies

```http
  GET /api/movies
```

#### Get movie

```http
  GET /api/movies/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### Update movie

```http
  PUT /api/movies/${id}
```

| Parameter  | Type     | Description                        |
| :--------- | :------- | :--------------------------------- |
| `id`       | `string` | **Required**. Id of item to fetch  |
| `isbn`     | `string` | request data                       |
| `title`    | `string` | request data                       |
| `director` | `json`   | request data (firstname, lastname) |

#### Create or add movie

```http
  POST /api/movies
```

| Parameter  | Type     | Description                                      |
| :--------- | :------- | :----------------------------------------------- |
| `isbn`     | `string` | **Required**. request data                       |
| `title`    | `string` | **Required**. request data                       |
| `director` | `json`   | **Required**. request data (firstname, lastname) |

#### Example JSON

```
{
    "isbn": "12345",
    "title": "One Piece",
    "director": {
        "firstname": "Ichiro",
        "lastname": "Odaa"
    }
}
```

## Authors

- [@bintangdilangit](https://www.github.com/bintangdilangit)

## Badges

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
