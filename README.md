# python-jquery-web-server
Old Fashioned, yet very simple web server with optional authentication


## Install
```bash
pip install -r requirements.txt
```

## Run
```bash
python3.6 backend/server.py 9999
```

## Run with Auth
```bash
python3.6 backend/server.py 9999 user:psw
```

## Backend
If you want your server to do more than just serve static files, go to `backend/routes.py` and add mappings.
E.g. 'dostuff: do_stuff'
This will map `localhost:9999/dostuff` with the `do_stuff` method which you then can implement in `backend/handler.py`.
