# super-simple-window

Create and return a Canvas within a JFrame using a bunch of optional settings and callbacks with one function.

## Installation

Add this to your Leiningen dependencies:

    [super-simple-window "0.0.1"]

## Usage

````clojure
(def -main []
  (new-super-simple-window {:title "Bad example"
                            :on-render my-render-fn
                            :on-key-press my-keypress-handler}))
````

 Create and return a Canvas within a JFrame using a bunch of optional settings and callbacks.
 A Timer is setup if :fps or :on-timer is given.
  Options:
    :title - Exactly what it sounds like. Defaults to \"Super simple window\".
    :width - The width of the Canvas within the window. Defaults to 640.
    :height - The height of the Canvas within the window. Defaults to 480.
    :fps - How often the timer (if used) runs. Defaults to 30.
    :on-timer - Callback that receives a ... object.
    :on-render - Callback that receives a Graphics object.
    :on-key-press - Callback that receives a KeyEvent object.

## License

Copyright © 2014 FIXME

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
