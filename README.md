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
* vertical
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/VerticalBarExample.png?raw=true)
    - Text for vertical bar
        ```html
        <ul class="stacked">
            <li>
                <span class="stacked-text"> (text)
                    <span class="subdued"> (subdued text) </span> (...)
                </span>
            </li>
        </ul>
        ```
* horizontal

    * bubble
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BubbleExample.png?raw=true "Bubble")
    * bar
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BarExample.png?raw=true "Bar")

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
   | :-----------:  | :-------------------------------: |
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

* Horizontal
    * Bubble Color:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BubbleColor.png?raw=true)

    * Bar Color:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/BarColor.png?raw=true)

* Vertical Color:
![alt text](https://github.com/maico910/css-progress-wizard/blob/maico910-patch-1/screenshots/VerticalBarColor.png?raw=true)

 |                           progress                        |                    text & icon color                    |        class        |
   | :-------------------------------------------------------- | :-------------------------------------------------------- | :------------------:|
   |  ![](https://placehold.it/15/65d074/000000?text=+)  green |  ![](https://placehold.it/15/65d074/000000?text=+)  green |    `completed `     |
   |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  |      `active`       |
   |  ![](https://placehold.it/15/5b32d6/000000?text=+) purple |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |       `info`        |
   |  ![](https://placehold.it/15/edb10a/000000?text=+) yellow |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      `warning`      |
   |  ![](https://placehold.it/15/d3140f/000000?text=+)  red   |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      `danger`       |
   |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  |      no class       |

```html
<ul class=(...)>  
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
- time
    ```html
    <div> (...)
        <span class="time"> (time) </span>
        (...)
    </div>
    ```

- sub-info
    ```html
    <div> (...)
        <span class="sub-info">
            <ul>
                <li> (sub-info)  </li>
                <li> (sub-info)  </li>  (...)
            </ul>
        </span>
    </div>
    ```    

### No Center Align
---
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
