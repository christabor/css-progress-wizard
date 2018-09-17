[![MIT Badge](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/christabor/css-progress-wizard/master/LICENSE)
![Donation badge](https://img.shields.io/gratipay/christabor.svg)

GITHUB https://github.com/christabor/css-progress-wizard

# A pure css progress indicator!
* Pure CSS (lightweight, easy to implement)
* Flexbox - easy to update and add more items
* Resizeable/responsive (text-resize, etc... try it!)
* Easy to customize design (sass mixins/variables, etc...)
* Written with SASS
----
### Progress Bar Format
*  Bar

        ul class="#"
   |     format    |              class                |
   | :-----------  | :------------------------------- |
   |     bubble    |         progress-indicator        |
   |      bar      | progress-indicator custom-complex |
   |  horizontal   |            (no class)             |
   |    vertical   |             stacked               |

*  Text for vertical bar

        <span class="stacked-text"> </span>

---
### Progress Color
    li class="#"

   |                           progress                        |                          text                            |        class        |
   | :-------------------------------------------------------- | :------------------------------------------------------- | :------------------:|
   |  ![](https://placehold.it/15/65d074/000000?text=+)  green | ![](https://placehold.it/15/65d074/000000?text=+) green  |     `completed `    |
   |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  | ![](https://placehold.it/15/337AB7/000000?text=+)  blue  |       `active`      |
   |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  | ![](https://placehold.it/15/bbb/000000?text=+)     gray  |       `info`        |
   |  ![](https://placehold.it/15/edb10a/000000?text=+) yellow | ![](https://placehold.it/15/edb10a/000000?text=+) yellow |      `warning`      |
   |  ![](https://placehold.it/15/edb10a/000000?text=+) yellow | ![](https://placehold.it/15/000000/000000?text=+) black  | `completed warning` |
   |  ![](https://placehold.it/15/337AB7/000000?text=+)  blue  | ![](https://placehold.it/15/bbb/000000?text=+)     gray  |   `completed info`  |
   |  ![](https://placehold.it/15/bbb/000000?text=+)     gray  | ![](https://placehold.it/15/bbb/000000?text=+)     gray  |       no class      |
> Black = default
---
## Time Line

    div id="timeline-speaker-example"
    span class="#" /span


- time
- sub-info
    ><ul>
        <li>   </li>
        <li>   </li>  (...)
    </ul>
---

### No center align
```
ul class="nocenter"
```
---


### Icons
```
<span class="fa fa-#"> </span>
```


   |     icon     |                                                               image                                                                |
   | :----------- | :--------------------------------------------------------------------------------------------------------------------------------: |
   | check-circle | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/check-circle.png "check-circle") |
   |    minus     | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/minus.png "minus")               |
   |  exclamation | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/exclamation.png "minus")         |
   |   calendar   | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/calendar.png "Calendar")         |
   |    comment   | ![alt text](https://raw.githubusercontent.com/maico910/css-progress-wizard/maico910-patch-1/icons/comment.png "comment")           |
