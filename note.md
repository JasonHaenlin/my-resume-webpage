# Example CV using the same css style classes

## Changes made in the CSS
```css
h1,
h2,
h3,
h4 {
    margin: 0;
}
```
## Classes added in the HTML without changing the HTML structure
```html
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <title>Example cv</title>
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
    <!-- HEADER -->
    <div class="header">
        <div class="header__title spacing-left">
            <h1 class="title bottom-border">MarianCorydon</h1>
        </div>
        <div class="header__profile spacing-left flex-container">
            <h2 class="header__profile__title flex-container--col1">mariancorydon1@gmail.com</h2>
        </div>
    </div>
    <!-- MAIN CONTENT -->
    <h2 class="spacing-left title header__description footer">Work Experience</h2>
    <span class="main item padding-around">
        <div class="item">
            <h3 class="item__title">Chemical Engineer</h3>
            <div class="item__detail">
                [text...]
            </div>
            <h3 class="item__title">Packaging Machine Operator</h3>
            <div class="item__detail">
                [text...]
            </div>
            <h3 class="item__title">Train Crew</h3>
            <div class="item__detail">
                [text...]
            </div>
            the<br>
            <h3 class="item__title ">Sciences Manager</h3>
            <div class="item__detail">
                [text...]
            </div>
        </div>
    </span>
    <h2 class="spacing-left title header__description footer">Education</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
    <h2 class="spacing-left title header__description footer">Skills</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
    <h2 class="spacing-left title header__description footer">Additional Information</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
</body>
</html>
```
## Classes added in the HTML after changing the HTML structure a little
```html
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <title>Example cv</title>
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
    <!-- HEADER -->
    <div class="header">
        <div class="header__title">
            <h1 class="title spacing-left bottom-border">MarianCorydon</h1>
        </div>
        <div class="header__profile">
            <h2 class="spacing-left">mariancorydon1@gmail.com</h2>
        </div>
    </div>
    <!-- MAIN CONTENT -->
    <h2 class="spacing-left title header__description footer">Work Experience</h2>
    <span class="main item padding-around">
<!-- here --><div class="container item item--left-line margin-around">
                <div class="item">
       <!-- here --><div class="timeline-circle"></div>
                    <h3 class="item__title spacing-left">Chemical Engineer</h3>
                    <div class="item__detail spacing-left">
                        [text...]
                    </div>
       <!-- here --><div class="timeline-circle"></div>
                    <h3 class="item__title spacing-left">Packaging Machine Operator</h3>
                    <div class="item__detail spacing-left">
                        [text...]
                    </div>
       <!-- here --><div class="timeline-circle"></div>
                    <h3 class="item__title spacing-left">Train Crew</h3>
                    <div class="item__detail spacing-left">
                        [text...]
                    </div>
       <!-- here --><div class="timeline-circle"></div>
                    <h3 class="item__title spacing-left">Sciences Manager</h3>
                    <div class="item__detail spacing-left">
                        [text...]
                    </div>
                </div>
<!-- here --></div>
    </span>
    <h2 class="spacing-left title header__description footer">Education</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
    <h2 class="spacing-left title header__description footer">Skills</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
    <h2 class="spacing-left title header__description footer">Additional Information</h2>
    <span class="main padding-around item__detail">
        [text...]
    </span>
</body>
</html>
```
