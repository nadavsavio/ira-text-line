# twilio-broadcast-plus
Local text-based broadcast service for neighborhood alerts. Adapted from Twilio's example function.

Twilio has a Function called "Twilio.org Tools: SMS Subscribe/Broadcast" that you can set to trigger on the "Incoming Messages" event. The function is a simple command handler that reacts to the first word of incoming texts:

`subscribe` --> adds the sender to the list of recipients

`unsubscribe` --> y'know

`broadcast [msg]` --> sends [msg] to all subscribed numbers | only works for admins (as defined in an environment variable)

This version of the code adds two commands:

`mods [msg]` --> sends [msg] only to admins 

`test [msg]` --> sends [msg] back to the number that sent it 
