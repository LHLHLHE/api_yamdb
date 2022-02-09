# YaMDb API
## Description
The YaMDb project collects user reviews on titles. The titles are divided into categories: "Books", "Movies", "Music". The list of categories can be expanded by the administrator (for example, you can add the category "Fine Art" or "Jewelry").
The titles themselves are not stored in YaMDb, you can't watch a movie or listen to music here.
A title can be assigned a genre from the preset list (for example, "Fairy Tale", "Rock" or "Arthouse"). Only the administrator can create new genres.
Grateful or outraged users leave text reviews for the titles and give the title a rating in the range from one to ten (an integer); an average rating of the title is formed from user ratings — a rating (an integer). The user can leave only one review for one title.

### Technologies
- Python 3.9.7
- Django 2.2.16
- Djangorestframework 3.12.4
- Redoc

### Launching a project in dev mode
- Install and activate the virtual environment
- Install dependencies from the file requirements.txt
    ```
    pip install -r requirements.txt
    ``` 
- In the file folder manage.py run the command:
    ```
    python manage.py runserver
    ```

### Authors
Халяпин Лев(Me)
Швейников Андрей(https://github.com/xxxRichiexxx)
Юркин Максим(https://github.com/Zoltrix88)


***

# Designing
### ER-diagram
![ER-diagram](https://github.com/xxxRichiexxx/api_yamdb/blob/master/%D0%94%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D1%8F/ER-%D0%B4%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0.PNG)

### API resources
- auth: authentication
- users: user management
- titles: titles with information about them (title, year of release, category, etc.)
- categories: categories (types) of titles ("Movies", "Books", "Music")
- genres: genres of titles. One title can be linked to several genres
- reviews: reviews of titles. The review is tied to a specific title
- comments: comments on reviews. The comment is linked to a specific review

### Development plan
![Graph](https://github.com/xxxRichiexxx/api_yamdb/blob/master/%D0%94%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D1%8F/%D0%9F%D0%BB%D0%B0%D0%BD.PNG)

### License
MIT License

Copyright (c) 2021 Халяпин Лев

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.