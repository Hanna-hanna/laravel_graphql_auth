## Laravel GraphQL Auth

<div>
    <p>Clone project</p>
    <pre>git clone https://github.com/Hanna-hanna/laravel_graphql_auth.git</pre>
    <pre>cd laravel_graphql_auth</pre>
    <p>Install Requirements</p>
    <pre>composer install</pre>
    <p>Create new database on the local database tool like TablePlus</p>
    <p>Create file .env from env.example (on the root) and add info</p>
    <pre>
    DB_DATABASE=name_your_database
    DB_USERNAME=your_username
    DB_PASSWORD=your_password
    </pre>
    <p>Migrate Database</p>
    <pre>php artisan migrate</pre>
    <p>Set key for application</p>
    <pre>php artisan key:generate</pre>
    <p>Start project from your server or use local</p>
    <pre>php artisan serve</pre>
    <p>Check API in Postman</p>
    <p>Create user (method post)</p>
    <pre>
    http://localhost:8000/graphql
    </pre>
    <p>Body (GraphQl)</p>
    <pre>
    mutation {
      createUser(name: "John Doe", email: "john@example.com", password: "password123") {
        id
        name
        email
      }
    }
    </pre>
    <p>Login user(method post)</p>
    <pre>
    http://localhost:8000/graphql
    </pre>
    <p>Body (GraphQl)</p>
    <pre>
    mutation {
      login(email: "john@example.com", password: "password123") {
        id
        name
        email
      }
    }
    </pre>

</div>
