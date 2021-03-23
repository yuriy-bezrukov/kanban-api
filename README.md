# kanban-api

> npm i

> npm start


<details>
<summary> users localhost:3001/user/</summary> 
#### users  `localhost:3001/user/`

##### method: GET

response:

```json
{ "status": "success", "message": Card }
```

##### method: PUT

request:

```json
{
  "text": string,
  "columnId": number,
  "userId": number
}
```

response:

```json
{ "status": "success", "message": Card }
```

##### method: POST

request:

```json
{
  "id": number,
  "text": string,
  "columnId": number,
  "userId": number
}
```

response:

```json
{ "status": "success", "message": Card[] }
```

##### method: DELETE

request:

```json
{
  "id": number
}
```

response:

```json
{ "status": "success" }
```

</details>

---

<details>
<summary> columns  localhost:3001/column/</summary> 
####  columns  `localhost:3001/column/`

##### method: GET

response:

```json
{ "status": "success", "message": Column[] }
```

##### method: PUT

request:

```json
{
  "name": string
}
```

response:

```json
{ "status": "success", "message": Column }
```

##### method: POST

request:

```json
{
  "id": number,
  "name": string
}
```

response:

```json
{ "status": "success", "message": Column }
```

##### method: DELETE

request:

```json
{
  "id": number
}
```

response:

```json
{ "status": "success" }
```

</details>

---

<details>
<summary> users  localhost:3001/user/</summary> 
####  users  `localhost:3001/user/`

##### method: GET

response:

```json
{ "status": "success", "message": User[] }
```

##### method: PUT

request:

```json
{
  "login": string
}
```

response:

```json
{ "status": "success", "message": User }
```

##### method: POST

request:

```json
{
  "id": number,
  "login": string
}
```

response:

```json
{ "status": "success", "message": User }
```

##### method: DELETE

request:

```json
{
  "id": number
}
```

response:

```json
{ "status": "success" }
```

</details>

---

<details>
<summary>Models</summary>

#### User

```json
{
  "id": number,
  "login": string
}
```

#### Card

```json
{
  "id": number,
  "text": string,
  "userId": number,
  "columnId": number
}
```

#### column

```json
{
  "id": number,
  "name": string
}
```

</details>
