## Creating project

```django-admin startproject <project name>```

## Running a server

```python3 manage.py runserver```

## Creating an app inside the project

```python3 manage.py startapp <app name>```

## Creating an admin user
```python3 manage.py makemigration```
```python3 manage.py migrate```
```python3 manage.py createsuperuser```

Sample user1:-

username: subhra

password: pass@subhra12

Sample user2:-

username: test1

password: pass@subhra12

## Applying changes to Database
```python3 manage.py makemigration```
```python3 manage.py migrate```

## View SQL code of migrations
```python3 manage.py sqlmigrate <app name> <migration number>```

## Shell Commands
### Accessing python shell
```python3 manage.py shell```
### Getting list of all users
```User.objects.all()```
### Creating new Post
Method 1:-

```post_1 = Post(title='Blog 2', content='Second Post Content!', author_id=user.id)```
```post_1.save()```

Method 2:-

```user = User.objects.all()[0]```
```user.post_set.create(title='Blog title', content='Post Content!')```

### Getting all Posts under a User
```user = User.objects.all()[0]```
```user.post_set.all()```

<b>Register your models in the admin.py file in the app to show it up in the admin panel</b>