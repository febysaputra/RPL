# SIKEMA / SIIKMA

SIIKMA adalah pengembangan sistem dari SIKEMA. SIIKMA berfungsi untuk memfasilitasi para pelaku usaha dalam mengikuti event-event yang diadakan oleh KEMENPERIN, dan memfasilitasi KEMENPERIN untuk mmengorganisir event yang diadakan.

## Getting Started

### Requirement
Menggunakan bahasa pemrograman PHP dengan framework Yii 2.0. Database postgersql 10.

Install Yii 2.0. Dapat mengikuti link berikut https://www.yiiframework.com/doc/guide/2.0/en/start-installation

### Get Source Code
```
git clone https://github.com/febysaputra/RPL.git
```

### Setup database
1. Create database
2. Restore database
    Gunakan .backup yang terbaru

### Setup application
1. Copy .env.dist to .env
2. Setting .env
```
    # Framework
    # ---------
    YII_DEBUG =  true
    YII_ENV = production

    # Databases
    # ---------
    DB_DSN = pgsql:host={your host db};port=5432;dbname={your db name}
    DB_USERNAME = {your username}
    DB_PASSWORD = {your password}
    DB_TABLE_PREFIX = cms_

    # Urls
    # ----
    FRONTEND_URL = http://{your domain}/frontend/
    BACKEND_URL = http://{your domain}/backend/
    STORAGE_URL = http://{your domain}/storage/

    # Other
    # -----
    TIMEZONE = UTC
    LANGUAGE = en-US

    MAINTENANCE_MODE = false
    MAINTENANCE_MODE_MESSAGE = 'Sorry, perform technical works.'
    MAINTENANCE_MODE_TIME = '0000-00-00 00:00:00'

    FRONTEND_COOKIE_VALIDATION_KEY = p6NhZE8BQUpggXICYp2iaXfJTo_s-tff
    BACKEND_COOKIE_VALIDATION_KEY = pKIj8Y_y8xTWIWdGo42pRhVcdj6zKef0

    ADMIN_EMAIL = hanifaffandihartanto@gmail.com
    ROBOT_EMAIL = hanifaffandihartanto@gmail.com

    LINK_ASSETS = false

    # Disqus
    # ------
    SHORT_NAME = 

```
3. Install requirements 
```
composer install
```
4. Run aplication
```
php yii serve --docroot="@root"
```
5. Open application in your lovely browser
