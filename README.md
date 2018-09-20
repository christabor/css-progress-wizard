[![MIT Badge](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/christabor/css-progress-wizard/master/LICENSE)

![Donation badge](https://img.shields.io/gratipay/christabor.svg)

GITHUB https://github.com/christabor/css-progress-wizard

# A pure css progress indicator!

- Pure CSS (lightweight, easy to implement)

- Flexbox - easy to update and add more items

- Resizeable/responsive (text-resize, etc... try it!)

- Easy to customize design (sass mixins/variables, etc...)

- Written with SASS


## Table of contents

* [Bar & Progress Format](#bar-&-progress-format)

  * [Bar](#bar)
    * [Horizontal Bar](#horizontal-bar)
      * [Bubble](#bubble)
      * [Bar](#bar)
    * [Vertical Bar](#vertical-bar)
      * [Text & Subdued Text](#text-&-subdued-text)
  * [Bar Format Class](#bar-format-class)
  * [Progress Format Class](#progress-format-class)

* [Color](#color)

  * [Bubble](#bubble)
  * [Bar](#bar)
  * [Vertical Bar](#vertical-bar)
  * [Color Class](#color-classes)

* [Time Line](#time-line)

  * [Time & sub-info](#time-&-sub-info)

* [No Center Align](#no-center-align)

* [Icons](#icons)

* [Link to Example](#link-to-example)


## Bar & Progress Format [&#x219F;](#table-of-contents)

### Bar [&#x219F;](#table-of-contents)

#### Horizontal Bar [&#x219F;](#table-of-contents)

##### Bubble [&#x219F;](#table-of-contents)

![Bubble](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/Bubble.png)

<details><summary>Show this example code</summary>


```html
<ul class="progress-indicator">
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 1.
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 2.
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 3.
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 4.
    </li>
    <li>
        <span class="bubble"></span>
        Step 5.
    </li>
</ul>
```

</details>

* How to use:

  ```html
  <!-- bubble bar -->
  <ul class="progress-indicator">
  	<li> (...) </li>
  </ul>	
  ```


##### Bar [&#x219F;](#table-of-contents)

![Bar](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/Bar.png)

<details><summary>Show this example code</summary>


```html
<ul class="progress-indicator custom-complex">
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 1.
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <i class="fa fa-check-circle"></i>
        Step 2.
    </li>
    <li>
        <span class="bubble"></span>
        Step 3.
    </li>
    <li>
        <span class="bubble"></span>
        Step 4.
    </li>
    <li>
        <span class="bubble"></span>
        Step 5.
    </li>
</ul>
```

</details>

- How to use

  ```html
  <!--  bar -->
  <ul class="progress-indicator custom-complex">
      <li> (...) </li>
  </ul>
  ```



#### Vertical Bar

​	![Vertical](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/Vertical.png) 

<details><summary>Show this example code</summary>


```html
<!-- first bar -->
<ul class="progress-indicator stepped stacked">
    <li class="completed warning">
        <span class="bubble"></span>
        <span class="stacked-text">
            <span class="fa fa-calendar"></span> June 3rd, 2014
            <span class="subdued">/ Added a thing. <em>Pssst... I'm a link!</em>
            </span>
        </span>
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">
            <span class="fa fa-calendar"></span> May 21st, 2014
            <span class="subdued">/ Some stuff happened. It was amazing.</span>
        </span>
    </li>
</ul>

<!-- second bar -->
<ul class="progress-indicator stepped stacked">
    <li class="completed info">
        <span class="bubble"></span>
        <span class="stacked-text">
            <span class="fa fa-calendar"></span> June 3rd, 2014
            <span class="subdued">/ Added a thing. <em>Pssst... I'm a link!</em></span>
        </span>
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">
            <span class="fa fa-calendar"></span> May 21st, 2014
            <span class="subdued">/ Some stuff happened. It was amazing.</span>
        </span>
    </li>
</ul>
```

</details>

- How to use:

  ```html
  <!-- vertical bar -->
  <ul class="stacked">
  	<li>(...)</li>
  </ul>
  ```




##### Text & Subdued Text

![VerticalText](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/VerticalText.png)

<details><summary>Show this example code</summary>


```HTML
<ul class="progress-indicator stepped stacked">
    <li class="completed warning">
        <span class="bubble"></span>
        <span class="stacked-text">
            I'm stacked-text
            <span class="subdued">/I'm a subdued text 1</span>
        </span>
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">
            I'm stacked-text 2
            <span class="subdued">
                <br>
                I'm a subdued text with line break</span>
        </span>
    </li>
</ul>
```

</details>

How to use [&#x219F;](#table-of-contents)

```html
<li>
    <span class="stacked-text">
        <!-- put here text -->
        I'm stacked-text 1
        <span class="subdued">
            <!-- put here subdued text  -->
            /I'm a subdued text 1 		
        </span>
    </span>
</li>
```

### Bar Format Class [&#x219F;](#table-of-contents)

|   format   |   class    |
| :--------: | :--------: |
| horizontal | (no class) |
|  vertical  |  stacked   |

```html
<!-- replace "x" to one of the classes -->
<ul class="x">
     <li> (...) </li>
</ul>
```

### Progress Format Class

| format |               class               |
| :----: | :-------------------------------: |
| bubble |        progress-indicator         |
|  bar   | progress-indicator custom-complex |

```html
<!-- replace x with one of the classes" -->
<li class=(...)>
    <span class="x"></span>
</li>
```

## Color [&#x219F;](#table-of-contents)

### Bubble [&#x219F;](#table-of-contents)

![BubbleColor](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/BubbleColor.png)

<details><summary>Show this example code</summary>
```html
<ul class="progress-indicator">
	<li class="completed">
        <span class="bubble"></span>
            green<br>
            (completed)
     </li>
    <li class="active">
        <span class="bubble"></span>
            blue<br>
            (active)
    </li>
    <li class="info">
        <span class="bubble"></span>
            purple<br>
            (info)
    </li>
    	<li class="warning">
        <span class="bubble"></span>
            yellow<br>
            (warning)
     </li>
    <li class="danger">
        <span class="bubble"></span>
            red<br>
            (danger)
    </li>
    <li>
        <span class="bubble"></span>
            gray<br>
            no class
    </li>
</ul>
```
</details>

### Bar [&#x219F;](#table-of-contents)

![BarColor](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/BarColor.png)

<details><summary>Show vertical bar example code</summary
```html
<ul class="progress-indicator custom-complex">
    <!-- green color -->
	<li class="completed">
        <span class="bubble"></span>
            green<br>
            (completed)
     </li>
    <!-- blue color -->
    <li class="active">
        <span class="bubble"></span>
            blue<br>
            (active)
    </li>
    <!-- purple color -->
    <li class="info">
        <span class="bubble"></span>
            purple<br>
            (info)
    </li>
    <!-- yellow color -->
    <li class="warning">
        <span class="bubble"></span>
            yellow<br>
            (warning)
     </li>
    <!-- red color -->
    <li class="danger">
        <span class="bubble"></span>
            red<br>
            (danger)
    </li>
    <!-- gray color -->
    <li>
        <span class="bubble"></span>
            gray<br>
            no class
    </li>
</ul>
```
</details>

### Vertical Bar [&#x219F;](#table-of-contents)

![VerticalColor](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/VerticalColor.png)

<details><summary>Show this example code</summary>
```html
<!-- fisrt bar -->
<ul class="progress-indicator stepped stacked">
    <!-- green color -->
	<li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">
            green<br>
            (completed)
        </span>
     </li>
    <!-- blue color -->
    <li class="active">
        <span class="bubble"></span>
        <span class="stacked-text">
            blue<br>
            (active)
        </span>
    </li>
    <!-- purple color -->
    <li class="info">
        <span class="bubble"></span>
        <span class="stacked-text">
            purple<br>
            (info)</span>
    </li>
</ul>

<!-- second bar -->
<ul class="progress-indicator stepped stacked">
    <!-- yellow color -->
    <li class="warning">
        <span class="bubble"></span>
        <span class="stacked-text">
            yellow<br>
            (warning)</span>
    </li>
    <!-- red color -->
    <li class="danger">
        <span class="bubble"></span>
        <span class="stacked-tex">
            red<br>
            (danger)
        </span>
    </li>
    <!-- gray color -->
    <li class="">
        <span class="bubble"></span>
        <span class="stacked-text">
            (gray)<br>
            no classe
        </span>
    </li>
</ul>
```
</details>

### Color Class [&#x219F;](#table-of-contents)

| progress                                                    | text & icon color                                           | class       |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------- |
| ![img](https://placehold.it/15/65d074/000000?text=+)  green | ![img](https://placehold.it/15/65d074/000000?text=+)  green | `completed` |
| ![img](https://placehold.it/15/337AB7/000000?text=+)  blue  | ![img](https://placehold.it/15/337AB7/000000?text=+)  blue  | `active`    |
| ![img](https://placehold.it/15/5b32d6/000000?text=+) purple | ![img](https://placehold.it/15/bbb/000000?text=+)     gray  | `info`      |
| ![img](https://placehold.it/15/edb10a/000000?text=+) yellow | ![img](https://placehold.it/15/bbb/000000?text=+)     gray  | `warning`   |
| ![img](https://placehold.it/15/d3140f/000000?text=+)  red   | ![img](https://placehold.it/15/bbb/000000?text=+)     gray  | `danger`    |
| ![img](https://placehold.it/15/bbb/000000?text=+)     gray  | ![img](https://placehold.it/15/bbb/000000?text=+)     gray  | no class    |

```html
<!-- horizontal or vertical bar -->
<ul class="(...)">
    <!-- replace x with one of the classes" -->
    <li class="x"> 
        (...)
    </li>
</ul>
```

## Time Line [&#x219F;](#table-of-contents)

![Time Line](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/TimeLine.png)

<details><summary>Show this example code</summary>
```html
<!-- class for time line -->
<div id="timeline-speaker-example">
    <h4>How about a speaker timeline?</h4>
    <ul class="progress-indicator stacked dark">
        <li class="current-time">
            <span class="time">I'm time</span>
            <span class="bubble"></span>
            <span class="stacked-text">
                I'm stacked-text
                <span class="subdued">I'm subdued</span>
                <span class="sub-info">
                    <ul>
                        <li>I'm sub-info</li>
                        <li>Second sub-info</li>
                        <li>Last sub-info</li>
                    </ul>
                </span>
            </span>
        </li>
        <li>
            <span class="time">1:30 - 2:30</span>
            <span class="bubble"></span>
            <span class="stacked-text">
                Some really cool title
                <span class="subdued">By a special speaker</span>
            </span>
        </li>
    </ul>
</div>
```
</details>

- How to use:

  ```html
  <div id="timeline-speaker-example">
      (...)
  </div>
  ```

### Time & sub-info [&#x219F;](#table-of-contents)

```html
<div> (...)
    <!-- put time here -->
    <span class="time"> (time) </span>
    <span class="sub-info">
        <ul>
            <!-- put sub-info here -->
            <li>I'm sub-info</li>
            <li>Second sub-info</li>
            <li>Last sub-info</li>
        </ul>
        (...)
    </span>
</div>
```

## No Center Align [&#x219F;](#table-of-contents)

![NoCenter](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/NoCenter.png)

<details><summary>Show this example code</summary>
```html
<!-- class for no center align -->
<ul class="progress-indicator nocenter stacked">
    <li class="completed info">
        <span class="bubble"></span>
        <span class="stacked-text">NO CENTER</span>
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">NO CENTER</span>
    </li>
    <li class="completed">
        <span class="bubble"></span>
        <span class="stacked-text">NO CENTER</span>
    </li>
</ul>
```
</details>

- How to use:

  ```html
  <ul class="nocenter">
  	(...)
  </ul>
  ```

## Icons [&#x219F;](#table-of-contents)

Font Awesome Icons.

![Icons](/home/michael910/Documents/Bibliotecas/Barra de Etapas/FlexProgressBar/screenshots/Icons.png)

<details><summary>Show this example code</summary>
```html
<ul class="progress-indicator ">
    <li class="completed">
        <span class="bubble"></span>
        <!-- check-circle icon  -->
        <span class="fa fa-check-circle"></span>
        check-cicle
    </li>
    <li class="active">
        <span class="bubble"></span>
        <!-- minus icon -->
        <span class="fa fa-minus"></span>
        active
    </li>
    <li class="info">
        <span class="bubble"></span>
        <!-- exclamation icon  -->
        <span class="fa fa-exclamation"></span>
        exclamation
    </li>
    <li class="warning">
        <span class="bubble"></span>
        <!-- calendar icon -->
        <span class="fa fa-calendar"></span>
        calendar
    </li>
    <li class="danger">
        <span class="bubble"></span>
        <!-- comment icon -->
        <span class="fa fa-comment"></span>
        comment
    </li>
</ul>
```
</details>

| class        | image                                                        |
| ------------ | ------------------------------------------------------------ |
| check-circle | ![img](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/check-circle.png) |
| minus        | ![img](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/minus.png) |
| exclamation  | ![img](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/exclamation.png) |
| calendar     | ![img](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/calendar.png) |
| comment      | ![img](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/comment.png) |

```html
<ul>
    <li>
        <!-- replace "x" for one of the classes -->
        <span class="fa fa-x"> </span> 
    </li>
</ul>
```

## Link to Example [&#x219F;](#table-of-contents)

[http://christabor.github.io/css-progress-wizard/](http://christabor.github.io/css-progress-wizard/ "Css Progress Wizard")
