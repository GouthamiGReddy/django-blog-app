# Django Blog App

A minimal Django blog with full CRUD (Create, Read, Update, Delete) for posts.

## Setup & Run

```bash
# 1. Install Django
pip install -r requirements.txt

# 2. Run migrations
python manage.py migrate

# 3. Start the dev server
python manage.py runserver
```

Then open http://127.0.0.1:8000 in your browser.

## Project Structure

```
blog_app/
├── manage.py
├── requirements.txt
├── blog_project/
│   ├── settings.py
│   └── urls.py
└── blog/
    ├── models.py      # Post model
    ├── views.py       # CRUD views
    ├── forms.py       # PostForm
    ├── urls.py        # URL routing
    └── templates/blog/
        ├── base.html
        ├── post_list.html
        ├── post_detail.html
        ├── post_form.html
        └── post_confirm_delete.html
```

## Features

- List all posts
- View a single post
- Create a new post
- Edit an existing post
- Delete a post (with confirmation)
