# super-simple-window

Create and return a Canvas within a JFrame using a bunch of optional settings and callbacks with one function.

## Installation

In Leiningen:

````clojure
    [super-simple-window "0.1.0"]
````

## Usage

There's just one function, `new-super-simple-window`.

````clojure
(new-super-simple-window {:title "Bad example"
                          :on-render my-render-fn
                          :on-key-press my-keypress-handler}))
````

 Create and return a Canvas within a JFrame using a bunch of optional settings and callbacks.
 A Timer is setup if :fps or :on-timer is given.
  Options:
<table>
  <tr><td>:title</td>
      <td>Exactly what it sounds like. Defaults to \"Super simple window\".</td></tr>
  <tr><td>:width</td>
      <td>The width of the Canvas within the window. Defaults to 640.</td></tr>
  <tr><td>:height</td>
      <td>The height of the Canvas within the window. Defaults to 480.</td></tr>
  <tr><td>:fps</td>
      <td>How often the timer (if used) runs. Defaults to 30.</td></tr>
  <tr><td>:on-timer</td>
      <td>Callback that receives a ... object.</td></tr>
  <tr><td>:on-render</td>
      <td>Callback that receives a Graphics object.</td></tr>
  <tr><td>:on-key-press</td>
      <td>Callback that receives a KeyEvent object.</td></tr>
</table>

## License

Copyright © 2014 Trystan

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
