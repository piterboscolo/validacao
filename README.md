# Validacao de Formulários com Express e EJS

**Bases do Projeto**

```
npm install
```

```
npm install express --save
```

```
npm install body-parser --save
```

```
npm install express-session --save
```

```
npm install ejs --save
```

```
npm install express-flash --save
```

**Express/Connect**

https://www.npmjs.com/package/body-parser

```
// parse application/x-www-form-urlencoded
app.use(bodyParser.urlencoded({ extended: false }))

// parse application/json
app.use(bodyParser.json())
```

https://www.npmjs.com/package/express-session

```
var app = express()
app.set('trust proxy', 1) // trust first proxy
app.use(session({
  secret: 'keyboard cat',
  resave: false,
  saveUninitialized: true,
  cookie: { secure: true }
}))
```

https://www.npmjs.com/package/flash

```
app.use(flash());
```



**Validação.js**

Uma biblioteca de validadores e sanitizadores de strings.

https://www.npmjs.com/package/validator
