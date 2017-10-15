# edc-notebooks
    
## Tunnel to DB

If your database is not on port 3306 ...

Open a tunnel to the live DB:

    ssh -f <user>@<server> -L5002:localhost:3306 -N


## Database conf

If you are running the notebook server in your project environment, you can just use the default database connection

Change the mysql settings (e.g. in your `/etc/<project>/mysql.conf`):

    port: 5002
    name: <database name>
    user: <readonly user>
    password: <password>

and then point to your settings file:

    python manage.py shell_plus --notebook --settings=<my_project>.settings

If you do not need to load models for the notebook then a simpler approach is to just reuse the database connection by setting `edc_notebook.settings`.DB_CONFIG to the correct path to `mysql.conf`.

        python manage.py shell_plus --notebook --settings=edc_notebook.settings
