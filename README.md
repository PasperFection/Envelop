# .env bestand om geheime omgevingsvariabelen te beheren voor applicaties
Dit bestand bevat alle omgevingsvariabelen die worden gebruikt door de applicatie.
Zorg ervoor dat je dit bestand veilig bewaart en niet deelt met onbevoegden door deze in een .env bestand te plaatsen.


```bash
## Algemene Instellingen

# Applicatie naam
# De naam van de applicatie die wordt gebruikt in verschillende delen van de app.
APP_NAME=MyApp

# Applicatie omgeving (production, development, etc.)
# Geeft aan in welke omgeving de applicatie draait. Dit kan bijvoorbeeld 'production' of 'development' zijn.
APP_ENV=production

# Applicatie sleutel voor encryptie
# Een unieke sleutel die wordt gebruikt voor het versleutelen van gegevens binnen de applicatie.
APP_KEY=base64:exampleKey1234567890exampleKey1234567890=

# Debug modus aan/uit
# Bepaalt of de debug modus is ingeschakeld. Dit kan helpen bij het oplossen van problemen tijdens de ontwikkeling.
APP_DEBUG=false

# Tijdzone van de applicatie
# De tijdzone waarin de applicatie draait. Dit kan invloed hebben op tijdgerelateerde functies.
APP_TIMEZONE=America/New_York

# URL van de applicatie
# De basis-URL van de applicatie. Dit wordt gebruikt voor het genereren van links en om de applicatie te bereiken.
APP_URL=https://myapp.example.com

# Standaard taal van de applicatie
# De standaardtaal die wordt gebruikt in de applicatie.
APP_LOCALE=en

# Fallback taal als de standaard taal niet beschikbaar is
# De taal die wordt gebruikt als de standaardtaal niet beschikbaar is.
APP_FALLBACK_LOCALE=en

# Faker locale voor het genereren van testdata
# De locale die wordt gebruikt door de Faker-bibliotheek om testdata te genereren.
APP_FAKER_LOCALE=en_US

## Onderhoudsinstellingen

# Onderhoudsmodus driver (file, database, etc.)
# De driver die wordt gebruikt om de onderhoudsmodus te beheren.
APP_MAINTENANCE_DRIVER=file

# Onderhoudsmodus opslag (optioneel, uitgeschakeld)
# Optionele instelling voor het opslaan van onderhoudsmodusgegevens.
APP_MAINTENANCE_STORE=database

## PHP Instellingen

# Aantal PHP CLI server workers
# Het aantal workers dat wordt gebruikt door de PHP CLI server.
PHP_CLI_SERVER_WORKERS=4

# Aantal Bcrypt rondes voor hashing
# Het aantal rondes dat wordt gebruikt door het Bcrypt-algoritme voor het hashen van wachtwoorden.
BCRYPT_ROUNDS=12

## Log Instellingen

# Log kanaal (stack, single, etc.)
# Het kanaal dat wordt gebruikt voor het loggen van berichten.
LOG_CHANNEL=stack

# Log stack type
# Het type stack dat wordt gebruikt voor het loggen.
LOG_STACK=single

# Log kanaal voor deprecations (uitgeschakeld)
# Het kanaal dat wordt gebruikt voor het loggen van verouderde functies.
LOG_DEPRECATIONS_CHANNEL=null

# Log niveau (debug, info, notice, etc.)
# Het niveau van logberichten dat wordt vastgelegd.
LOG_LEVEL=info

## Database Instellingen

# Database URL
# De URL die wordt gebruikt om verbinding te maken met de database.
DATABASE_URL=pgsql://exampleUser:examplePassword@db.example.com:5432/exampleDB

# Database verbindingstype
# Het type verbinding dat wordt gebruikt voor de database.
DB_CONNECTION=pgsql

# Database host
# De hostnaam of het IP-adres van de database server.
DB_HOST=db.example.com

# Database poort
# De poort die wordt gebruikt om verbinding te maken met de database.
DB_PORT=5432

# Database naam
# De naam van de database.
DB_DATABASE=exampleDB

# Database gebruikersnaam
# De gebruikersnaam die wordt gebruikt om verbinding te maken met de database.
DB_USERNAME=exampleUser

# Database wachtwoord
# Het wachtwoord dat wordt gebruikt om verbinding te maken met de database.
DB_PASSWORD=examplePassword

# Database karakterset
# De karakterset die wordt gebruikt door de database.
DB_CHARSET=utf8

# Database prefix voor tabellen
# Een optionele prefix die wordt toegevoegd aan alle tabelnamen in de database.
DB_PREFIX=

# Database prefix voor indexen
# Een optionele prefix die wordt toegevoegd aan alle indexnamen in de database.
DB_PREFIX_INDEXES=true

# Database zoekpad
# Het zoekpad dat wordt gebruikt door de database.
DB_SEARCH_PATH=public

# Database SSL modus
# De SSL-modus die wordt gebruikt voor de databaseverbinding.
DB_SSLMODE=require

## Sessie Instellingen

# Sessie driver (file, database, etc.)
# De driver die wordt gebruikt voor het beheren van sessies.
SESSION_DRIVER=database

# Sessie levensduur in minuten
# De levensduur van een sessie in minuten.
SESSION_LIFETIME=120

# Sessie encryptie aan/uit
# Bepaalt of sessies worden versleuteld.
SESSION_ENCRYPT=false

# Sessie pad
# Het pad dat wordt gebruikt voor sessies.
SESSION_PATH=/

# Sessie domein (optioneel)
# Het domein dat wordt gebruikt voor sessies.
SESSION_DOMAIN=null

## Broadcasting Instellingen

# Broadcast verbindingstype
# Het type verbinding dat wordt gebruikt voor broadcasting.
BROADCAST_CONNECTION=log

## Filesystem Instellingen

# Filesystem schijf
# De schijf die wordt gebruikt voor het opslaan van bestanden.
FILESYSTEM_DISK=local

## Queue Instellingen

# Queue verbindingstype
# Het type verbinding dat wordt gebruikt voor queues.
QUEUE_CONNECTION=database

## Cache Instellingen

# Cache opslag
# De opslag die wordt gebruikt voor caching.
CACHE_STORE=database

# Cache prefix
# Een optionele prefix die wordt toegevoegd aan alle cache sleutels.
CACHE_PREFIX=

## Memcached Instellingen

# Memcached host
# De hostnaam of het IP-adres van de Memcached server.
MEMCACHED_HOST=127.0.0.1

## Redis Instellingen

# Redis client
# De client die wordt gebruikt voor Redis.
REDIS_CLIENT=phpredis

# Redis host
# De hostnaam of het IP-adres van de Redis server.
REDIS_HOST=127.0.0.1

# Redis wachtwoord (optioneel)
# Het wachtwoord dat wordt gebruikt om verbinding te maken met de Redis server.
REDIS_PASSWORD=null

# Redis poort
# De poort die wordt gebruikt om verbinding te maken met de Redis server.
REDIS_PORT=6379

## Mail Instellingen

# Mailer type
# Het type mailer dat wordt gebruikt voor het verzenden van e-mails.
MAIL_MAILER=smtp

# Mail host
# De hostnaam of het IP-adres van de mailserver.
MAIL_HOST=smtp.example.com

# Mail poort
# De poort die wordt gebruikt om verbinding te maken met de mailserver.
MAIL_PORT=587

# Mail gebruikersnaam
# De gebruikersnaam die wordt gebruikt om verbinding te maken met de mailserver.
MAIL_USERNAME=example@example.com

# Mail wachtwoord
# Het wachtwoord dat wordt gebruikt om verbinding te maken met de mailserver.
MAIL_PASSWORD=examplePassword

# Mail encryptie type
# Het type encryptie dat wordt gebruikt voor de mailverbinding.
MAIL_ENCRYPTION=tls

# Mail van adres
# Het e-mailadres dat wordt gebruikt als afzender.
MAIL_FROM_ADDRESS="no-reply@example.com"

# Mail van naam
# De naam die wordt gebruikt als afzender.
MAIL_FROM_NAME="MyApp"

## AWS Instellingen

# AWS toegangssleutel ID
# De toegangssleutel ID die wordt gebruikt voor AWS.
AWS_ACCESS_KEY_ID=exampleAccessKeyId

# AWS geheime toegangssleutel
# De geheime toegangssleutel die wordt gebruikt voor AWS.
AWS_SECRET_ACCESS_KEY=exampleSecretAccessKey

# AWS standaard regio
# De standaardregio die wordt gebruikt voor AWS.
AWS_DEFAULT_REGION=us-east-1

# AWS bucket naam
# De naam van de AWS bucket die wordt gebruikt.
AWS_BUCKET=exampleBucket

# AWS gebruik padstijl endpoint aan/uit
# Bepaalt of padstijl endpoints worden gebruikt voor AWS.
AWS_USE_PATH_STYLE_ENDPOINT=false

## Vite Instellingen

# Vite applicatie naam
# De naam van de Vite applicatie.
VITE_APP_NAME="MyApp"

## Supabase Instellingen

# Supabase URL
# De URL die wordt gebruikt om verbinding te maken met Supabase.
SUPABASE_URL=https://example.supabase.co

# Supabase anonieme sleutel
# De anonieme sleutel die wordt gebruikt voor Supabase.
SUPABASE_ANON_KEY=exampleAnonKey1234567890exampleAnonKey1234567890

## E-mail Instellingen

# E-mail host
# De hostnaam of het IP-adres van de e-mailserver.
EMAIL_HOST=smtp.mailersend.net

# E-mail poort
# De poort die wordt gebruikt om verbinding te maken met de e-mailserver.
EMAIL_PORT=587

# E-mail beveiliging aan/uit
# Bepaalt of de e-mailverbinding beveiligd is.
EMAIL_SECURE=false

# E-mail gebruikersnaam
# De gebruikersnaam die wordt gebruikt om verbinding te maken met de e-mailserver.
EMAIL_USER=exampleUser@trial.example.com

# E-mail wachtwoord
# Het wachtwoord dat wordt gebruikt om verbinding te maken met de e-mailserver.
EMAIL_PASS=examplePassword

## JWT Instellingen

# JWT geheime sleutel
# De geheime sleutel die wordt gebruikt voor JWT (JSON Web Token) authenticatie.
JWT_SECRET=exampleSecretKey

# JWT algemene levensduur
# De algemene levensduur van een JWT in seconden.
JWT_TTL=3600

# JWT verversing levensduur
# De levensduur van een JWT verversingstoken in seconden.
JWT_REFRESH_TTL=86400

## Mailer Verzender Instellingen

# Mailer verzender API key
# De API sleutel die wordt gebruikt door de mailer verzender.
MAILERSEND_API_KEY=exampleApiKey

# Mailer verzender naam
# De naam die wordt gebruikt door de mailer verzender.
MAILERSEND_FROM_NAME=MyApp

# Mailer verzender email
# Het e-mailadres dat wordt gebruikt door de mailer verzender.
MAILERSEND_FROM_EMAIL=example@example.com

## Node.js Instellingen

# Node omgeving
# De omgeving waarin de Node.js applicatie draait.
NODE_ENV=production

## OpenAI Instellingen

# OpenAI API sleutel
# De API sleutel die wordt gebruikt om verbinding te maken met de OpenAI API.
OPENAI_API_KEY=exampleApiKey

# OpenAI organisatie
# De organisatie die wordt gebruikt voor de OpenAI API.
OPENAI_ORGANIZATION=exampleOrganization

# OpenAI model
# Het model dat wordt gebruikt door de OpenAI API.
OPENAI_MODEL=gpt-4o

# OpenAI temperatuur
# De temperatuur die wordt gebruikt door de OpenAI API voor het genereren van tekst.
OPENAI_TEMPERATURE=0.5

# OpenAI maximum aantal tokens
# Het maximum aantal tokens dat wordt gebruikt door de OpenAI API voor het genereren van tekst.
OPENAI_MAX_TOKENS=4000

# OpenAI top p
# De top-p parameter die wordt gebruikt door de OpenAI API voor het genereren van tekst.
OPENAI_TOP_P=1

# OpenAI frequentie penalty
# De frequentie penalty die wordt gebruikt door de OpenAI API voor het genereren van tekst.
OPENAI_FREQUENCY_PENALTY=0

# OpenAI aanwezigheid penalty
# De aanwezigheid penalty die wordt gebruikt door de OpenAI API voor het genereren van tekst.
OPENAI_PRESENCE_PENALTY=0

# OpenAI API URL
# De URL die wordt gebruikt om verbinding te maken met de OpenAI API.
OPENAI_API_URL=https://api.openai.com/v1

# OpenAI API type
# Het type API dat wordt gebruikt door OpenAI.
OPENAI_API_TYPE=openai

# OpenAI API versie
# De versie van de OpenAI API die wordt gebruikt.
OPENAI_API_VERSION=2024-02-15-preview

## Stripe Instellingen (optioneel, uitgeschakeld)

# Stripe publiceerbare sleutel (optioneel, uitgeschakeld)
# De publiceerbare sleutel die wordt gebruikt door Stripe. Dit is optioneel en kan worden uitgeschakeld.
STRIPE_PUBLISHABLE_KEY=examplePublishableKey

# Stripe geheime sleutel (optioneel, uitgeschakeld)
# De geheime sleutel die wordt gebruikt door Stripe. Dit is optioneel en kan worden uitgeschakeld.
STRIPE_SECRET_KEY=exampleSecretKey

## API Instellingen

# API rate limit
# Het maximum aantal API-aanvragen dat per tijdseenheid is toegestaan.
API_RATE_LIMIT=100
```

## .env bestand plaatsen
Plaats het .env bestand in de root van de applicatie.

## .env bestand laden
Voeg het .env bestand toe aan het .gitignore bestand zodat het niet wordt gepubliceerd naar de repository.

## .env bestand configureren
Configureer de omgevingsvariabelen in het .env bestand op basis van de vereisten van de applicatie.

## .env bestand gebruiken
Gebruik de omgevingsvariabelen in de applicatie door ze in de code te laden met de `env` functie.

### PHP & Laravel
```php
$value = env('VARIABLE_NAME');
```

### JavaScript / TypeScript & Node.js
```js
const value = process.env.VARIABLE_NAME;
```

### Bash & Linux
```bash
value=$(printenv VARIABLE_NAME)
```

### Python && Django
```python
value = os.getenv('VARIABLE_NAME')
```

### C# && .NET
```csharp
var value = Environment.GetEnvironmentVariable("VARIABLE_NAME");
```

### Ruby && Rails
```ruby
value = ENV['VARIABLE_NAME']
```

### Swift && iOS
```swift
let value = ProcessInfo.processInfo.environment["VARIABLE_NAME"]
```
