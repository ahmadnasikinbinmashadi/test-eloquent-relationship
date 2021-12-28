# Test Laravel Eloquent Relationships
This repository is My answers from a challenge of test eloquent relationship by **PovilasKorop** (https://github.com/LaravelDaily/Test-Eloquent-Relationships)

---

## Unit Testing

To running a laravel test, run `php artisan test` if you using windows, or `vendor/bin/phpunit` if you using linux .

---

## Points of test
There are 9 points of test

---

### 1. HasMany relationship.

In `app/Models/User.php` file

Test method `test_user_create_task()`.

---

### 2. BelongsTo with Empty Relationship.

In the route `/tasks`, int the table list, show listing all the tasks, just showing an empty space where the user name should have been.

Test method `test_task_with_no_user()`.

---

### 3. Two-level Relationship.

In the route `/users/{user}`, Definning a relationship from User to Comment in the User model, so that the table load the comments that are written on the task that belong to a user.

Test method `test_show_users_comments()`.

---

### 4. BelongsToMany - Pivot Table Name.

In the route `/roles`, Definning relationship in `app/Models/Role.php` model the table load the roles with the number of users belonging to them.

Test method `test_show_roles_with_users()`.

---

### 5. BelongsToMany - Extra Fields in Pivot Table.

In the route `/teams`, Definning a relationship in `app/Models/Team.php` so that the table show the teams with users, each user with a few additional fields.

Test method `test_teams_with_users()`.

---

### 6. HasMany - Average from Field Value

In the route `/countries`, Definning a relationship number so that the table show the countries with average team size.

Test method `test_countries_with_team_size()`.

---

### 7. Polymorphic Attachments

In the route `/attachments`, Definning a relationship in `app/Models/Attachment.php`  so that the table show the filenames and the class names of Task and Comment models.

Test method `test_attachments_polymorphic()`.

---

### 8. Add BelongsToMany Row

In the POST route `/projects`, save a project for a logged-in user, with start_date field from $request.

Test method `test_belongstomany_add()`.

---

### 9. Filter BelongsToMany Rows

In the route `/users`, Filter the user list that only the users with at least one project.

Test method `test_filter_users()`.

---

## Refference
Original repository (Github) :  https://github.com/LaravelDaily/Test-Eloquent-Relationships
Youtube: https://www.youtube.com/watch?v=ohj0Mc09DyE&list=PLdXLsjL7A9k2-4sY2rLgB89MQQK0QeHvs&index=6

