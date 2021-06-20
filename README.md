# PacketTracer Assessment Values
The purpose of this project is document assessment values for PacketTracer Activites. 

* [Switch Assessment Values](/Switch_Value_Guide.md) (work in progress)
* [Router Assessment Values](/Router_Value_Guide.md) (haven't started this yet)
* [PC Assessment Values](/PC_Value_Guide.md) (work in progress)
* Wireless LAN Controller (haven't started this yet)

## Misc
### Regular Expressions for MOTD & Description values
#### Match anything, has to be at least one character
<pre>{{RegEx:.+}}</pre>
#### Matches the KEYWORD and anything character(s) before or after it.
<pre>{{RegEx:.*KEYWORD.*}}</pre>	
