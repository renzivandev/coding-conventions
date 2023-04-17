# coding-conventions
- 2 spaces tab
- no semicolon
- refrain from using h1-h6, ul, li, etc.
	- dont wanna waste time to remove the default margins/paddings
	- can be used on special cases, provided you can justify why
	- use div and span instead
- use only bootstrap utility classes as much as possible 
- 120 characters per line for template
- 80 characters per line for script
- for custom classes naming convention use BEM (https://getbem.com/)
	- Unless its necessary, you don't need to have a custom class for img, a, & span
	- Example:
    ```
    <template>
    <div class="header">
    <div class="header-title">
        This is the title
        <span>with some text</span>
        <span class="header-title__some-text">with some more text</span>
        <img src="" alt="" />
    </div>
    <div class="header-subtitle">with a subtitle</div>
    <div class="header-boxes">
        <div class="header-box header-box--red">box red</div>
        <div class="header-box header-box--green">box green</div>
        <div class="header-box header-box--blue">box blue</div>
    </div>
    </div>
    </template>
    <style lang="scss" scoped>
    .header {
        &-title {
            span {}

            img {}

            &__some-text {}
        }

        &-subtitle {}

        &-boxes {}

        &-box {
            &--red {}

            &--green {}

            &--blue {}
        }
    }
    </style>
    ```
- function space around parentheses
    - Example:
	```
    function test () {
      // function
    }
	```
- new line after a block
    - Example:
	```
    function test () {
      if (x === y) {
	    return x
      }

      return y
    }
	```

#### You might see some code that I violated this list, e.g. h5 in Modal, will fix this
