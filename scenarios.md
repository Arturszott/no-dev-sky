# Part 1

####scene 1

You woke up in the dark room. You can see some flashing lights on the metal wall. There is some box in the middle.

You can't remember anything. 

Who are you?

>>Get up and take a look at the table.


####scene 2

On the top of the box lays down the device. You read: **State Device**, not bad!. There is also warning card: _Use with caution. Risk of data discrepancy!_. It can be useful, so you pick it up.

>>Check the wall with flashing lights


####scene 3

Next to the panel with some diodes you've spotted the door. They don't have any doorknobs. Where are you?
Only three of six lights are blinking. Why? With your bare hands you've managed to open the panel. 

Underneath you see the following component. Maybe it's the right time to use your new device?

```javascript
var DoorOpener = React.createClass({
  getInitialState: function() {
    return {
      s1: true, s2: true, s3: undefined, s5: false, s6: true
    }
  },

  render: function() {
    var state = this.state;
    var combination = state.s1 === (state.s2 !== state.s4) && state.s6 === (state.s3 !== state.s5);
    
    return <Door isOpened={combination} />
  }
});
```

# Part 2

You hear some clicks and the door is slowly opening...
