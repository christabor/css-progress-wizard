[![MIT Badge](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/christabor/css-progress-wizard/master/LICENSE)
![Donation badge](https://img.shields.io/gratipay/christabor.svg)

GITHUB https://github.com/christabor/css-progress-wizard

# A pure css progress indicator!
---
* Pure CSS (lightweight, easy to implement)
* Flexbox - easy to update and add more items
* Resizeable/responsive (text-resize, etc... try it!)
* Easy to customize design (sass mixins/variables, etc...)
* Written with SASS

## Introduction
---
* Progress Format
* Bar Format
* Color
* Time Line
* No Center Align
* Font Awesome Icons
* Link to Exampple


### Bar & Progress Format
---
##### Vertical Bar:

![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/VerticalBarExample.png?raw=true)

```html
        <ul class="progress-indicator stepped stacked">
            <li class="completed warning">
                <a href="#">
                    <span class="bubble"></span>
                    <span class="stacked-text">
                        <span class="fa fa-calendar"></span> June 3rd, 2014
                        <span class="subdued">/ Added a thing. <em>Pssst... I'm a link!</em></span>
                    </span>
                </a>
            </li>
            <li class="completed">
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> May 21st, 2014
                    <span class="subdued">/ Some stuff happened. It was amazing.</span>
                </span>
            </li>
            <li>
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> April 11th, 2014
                    <span class="subdued">/ What a wild day!</span>
                </span>
            </li>
            <li>
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> February 3rd, 2014
                    <span class="subdued">/ This day is toooo long.</span>
                </span>
            </li>
            <li>
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-comment"></span> January 5th, 2014
                    <span class="subdued">/ Happy birthday, me!</span>
                </span>
            </li>
        </ul>
        <ul class="progress-indicator stepped stacked">
            <li class="completed info">
                <a href="#">
                    <span class="bubble"></span>
                    <span class="stacked-text">
                        <span class="fa fa-calendar"></span> June 3rd, 2014
                        <span class="subdued">/ Added a thing. <em>Pssst... I'm a link!</em></span>
                    </span>
                </a>
            </li>
            <li class="completed">
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> May 21st, 2014
                    <span class="subdued">/ Some stuff happened. It was amazing.</span>
                </span>
            </li>
            <li class="completed">
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> April 11th, 2014
                    <span class="subdued">/ What a wild day!</span>
                </span>
            </li>
            <li class="completed">
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-calendar"></span> February 3rd, 2014
                    <span class="subdued">/ This day is toooo long.</span>
                </span>
            </li>
            <li>
                <span class="bubble"></span>
                <span class="stacked-text">
                    <span class="fa fa-comment"></span> January 5th, 2014
                    <span class="subdued">/ Happy birthday, me!</span>
                </span>
            </li>
        </ul>
```


* Vertical Bar Text
    ```html
        <li>
            <span class="stacked-text">            
                <!-- put here text for progress -->     
                I'm stacked-text 1
            </span>
        </li>
    ```
* Vertical Bar Subdued Text
    ```html
    <li>
        <span class="stacked-text">
            (...)
                <span class="subdued">
                <!-- put here subdued text for progress -->
                /I'm a subdued text 1
            </span>
        </span>
    </li>
    ```
* Horizontal:
    * Bubble:
    ![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BubbleExample.png?raw=true "Bubble")
    ```html
    <ul class="progress-indicator">
        <li> (...) </li>
    </ul>
    ```

    * Bar:
    ![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BarExample.png?raw=true "Bar")
    ```html
    <ul class="progress-indicator custom-complex">
        <li> (...) </li>
    </ul>
    ```

* Bar Format:

   |     format    |    class   |
   | :-----------: | :--------: |
   |  horizontal   | (no class) |
   |   vertical    |   stacked  |

    ```html
    <ul class="x">    <!-- replace "x" to one of the classes -->
        <li> (...) </li>
    </ul>
    ```

* Progress Format:
    |     format    |              class                |
    | :-----------: | :-------------------------------: |
    |     bubble    |         progress-indicator        |
    |      bar      | progress-indicator custom-complex |
    ```html
    <li class=(...)>
        <span class="x">    <!-- replace x with one of the classes" -->
        </span>
    </li>
    ```

### Color
---

* Horizontal Bar Color Example:
    * Bubble:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BubbleColor.png?raw=true "Horizontal Bubble Color Example")
    * Bar:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BarColor.png?raw=true "Horizontal Bar Color Example")

    ```html
    <ul class="progress-indicator">   <!-- add "custom-complex for bar -->
        <li class="completed">
            <span class="bubble"></span> green
        </li>
        <li class="active">
            <span class="bubble"></span> blue
        </li>
        <li class="info">
            <span class="bubble"></span> purple
        </li>
        <li class="warning">
            <span class="bubble"></span> yellow
        </li>
        <li class="danger">
            <span class="bubble"></span> red
        </li>
        <li>
            <span class="bubble"></span> gray
        </li>
    </ul>
    ```

* Vertical Bar Color Example:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/VerticalBarColor.png?raw=true "Vertical Bar Color Example")
    ```html
    <ul class="progress-indicator stepped stacked">
        <li class="completed">
            <span class="bubble"></span>
            <span class="stacked-text">green</span>
        </li>
        <li class="active">
            <span class="bubble"></span>
            <span class="stacked-text">blue</span>
        </li>
        <li class="info">
            <span class="bubble"></span>
            <span class="stacked-text">purple</span>
        </li>
        <li class="completed">
            <span class="bubble"></span>
            <span class="stacked-text">green</span>
        </li>
        <li class="active">
            <span class="bubble"></span>
            <span class="stacked-text">blue</span>
        </li>
        <li class="info">
            <span class="bubble"></span>
            <span class="stacked-text">purple</span>
        </li>
    </ul>
    ```
* Color Classes
     |                           progress                        |                    text & icon color                    |        class        |
       | :-------------------------------------------------------- | :-------------------------------------------------------- | :------------------:|
       |  ![](https://placehold.it/15/65d074/000000?text=+)  green |  ![](https://placehold.it/15/65d074/000000?text=+)  green |    `completed `     |
       |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  |      `active`       |
       |  ![](https://placehold.it/15/5b32d6/000000?text=+) purple |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |       `info`        |
       |  ![](https://placehold.it/15/edb10a/000000?text=+) yellow |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      `warning`      |
       |  ![](https://placehold.it/15/d3140f/000000?text=+)  red   |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      `danger`       |
       |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      no class       |

    ```html
    <ul class=(...)>    <!-- horizontal or vertical bar -->
        <li class="x">  <!-- replace x with one of the classes" -->
            (...)
        </li>
    </ul>
    ```

### Time Line
---
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/TimeLine.png?raw=true)
```html
<div id="timeline-speaker-example">
    (...)
</div>
```
- time & sub-info
    ```html
    <div> (...)
        <span class="time"> (time) </span>
        <span class="sub-info">
            <ul>
                <li>I'm sub-info</li>
                <li>Second sub-info</li>
                <li>Last sub-info</li>
            </ul>
            (...)
        </span>
    </div>
    ```



### No Center Align
---
`IMAGEM` NO CENTER EXEMPLO
```html
<ul class="nocenter">
    (...)
</ul>
```

### Font Awesome Icons
---
   |     icon     |                                                               image                                                                |
   | :----------- | :--------------------------------------------------------------------------------------------------------------------------------: |
   | check-circle | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/check-circle.png "check-circle") |
   |    minus     | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/minus.png "minus")               |
   |  exclamation | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/exclamation.png "minus")         |
   |   calendar   | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/calendar.png "Calendar")         |
   |    comment   | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/comment.png "comment")           |

```html
<ul>
    <li>
        <span class="fa fa-x"> </span> <!-- replace "x" for one of the classes -->
    </li>
</ul>
```


### Link to Example
---
[http://christabor.github.io/css-progress-wizard/](http://christabor.github.io/css-progress-wizard/ "Css Progress Wizard")
