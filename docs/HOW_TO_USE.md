# How to use system

- Add app to your ```settings.py```
- Customize the user model according to your wishes
- Customize view files according to your own template files.

## Edit Settings

Add these to your settings file;

```python
MEDIA_URL = '/media/'
MEDIA_ROOT = os.path.join(BASE_DIR, 'media/')

AUTH_USER_MODEL = 'account.CustomUser'
LOGIN_REDIRECT_URL = '/'
```

## Migration

- Use
```python
python manage.py makemigrations
python manage.py migrate
```