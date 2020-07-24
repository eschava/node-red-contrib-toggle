# node-red-contrib-toggle
Toggle switch node for Node-red

This node could be a companion for any switch (physical or virtual), storing its state and providing "toggle" operation
without need of using function nodes or flow/global variables
  
## Usage

Super easy. Just provide payload for changing switch to ON/OFF state and one extra payload for toggling state of the switch.  
It's possible to specify "Any except ON/OFF" value that toggles switch state if incoming message is not ON or OFF.  

**Pass-through mode**  
Node has three pass-through modes:  
 - "No" means that node sends a message only when state is toggled. ON/OFF input messages just update internal state of the node.
 - "If changed" sends a message for ON/OFF input message only once it differs from the previous state. And obviously message is always sent for "toggle" message. 
 - "Always" - output message is always sent as a reaction on an input message


## Version history

v0.0.2 Docs updated

v0.0.1 Initial release

