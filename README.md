# 🌍 World Capitals Project (Express.js + PostgreSQL + EJS)


---

Do you want me to also **embed the EJS template code** (`index.ejs`) inside this same markdown page so it’s truly “all in one page”?

---

## 📷 Gallery

| Quizz| Quizz|
|--------|--------|
| ![pgq1](pgq1.png){style="border:2px solid #000;"} | ![pgq2](pgq2.png){style="border:2px solid #000;"} |

| Quizz |
|--------|
| <div style="text-align:center;"><img src="pgq3.png" style="border:2px solid #000;" /></div> |

---

## 1️⃣ Create Table in PostgreSQL
```sql
CREATE TABLE capitals1 (
    id SERIAL PRIMARY KEY,
    country VARCHAR(45),
    capital VARCHAR(45)
);
```
2️⃣ Install Dependencies
```bash
npm i
npm i pg express ejs body-parser
```

3️⃣ Database Connection (index.js)
```bash
const app = express()
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "world",
  password: "XXXX",   // <-- your PostgreSQL password
  port: XXXX // <-- your PostgreSQL port number
})
```

4️⃣ Run Server
```bash
node index.js
```
