### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

Paragraph lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

* Bullet 1
* Bullet 2
* Bullet 3
* Bullet 4

1. Item 1
1. Item 2
1. Item 3

* `handlers.link` is fired with the result of each discovered link (broken or not) within the current queue item.
* `handlers.item` is fired after a queue item's last result, on zero results, or if the HTML could not be retreived.
* `handlers.end` is fired when the end of the queue has been reached.

* `.dequeue(id)` removes an item from the queue. Returns `true` on success or an `Error` on failure.
* `.enqueue(htmlUrl, customData)` adds an item to the queue. Items are auto-dequeued when their requests are complete. Returns a queue ID on success or an `Error` on failure.
  * `customData` is optional data that is stored in the queue item.
* `.length()` returns the number of items in the queue.
* `.numActiveItems()` returns the number of active HTML URL sessions (series of link requests).
* `.numActiveLinks()` returns the number of active link requests.
* `.pause()` will pause the queue, but will not pause any active requests.
* `.resume()` will resume the queue.
