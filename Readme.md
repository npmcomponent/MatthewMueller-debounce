
# debounce

  Underscore's debounce method as a component.

  Creates and returns a new debounced version of the passed function that will postpone its execution until after wait milliseconds have elapsed since the last time it was invoked.

## Installation

    $ component install matthewmueller/debounce

## Example

  ```js
    var debounce = require('debounce');
    window.onresize = debounce(resize, 200);

    function resize(e) {
      console.log('height', window.innerHeight);
      console.log('width', window.innerWidth);
    }
  ```

## API

  ### debounce(fn, wait, [ immediate ])

  Creates and returns a new debounced version of the passed function that will postpone its execution until after wait milliseconds have elapsed since the last time it was invoked. Useful for implementing behavior that should only happen after the input has stopped arriving. For example: rendering a preview of a Markdown comment, recalculating a layout after the window has stopped being resized, and so on.

  Pass true for the immediate parameter to cause debounce to trigger the function on the leading instead of the trailing edge of the wait interval. Useful in circumstances like preventing accidental double-clicks on a "submit" button from firing a second time.

## License

  MIT