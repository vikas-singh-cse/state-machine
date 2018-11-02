State machines are very simple in C if you use function pointers.

Basically you need 2 arrays:
-> one for state function pointers and
-> one for state transition rules. 

Every state function returns the code, you lookup state transition table by state and return code to find the
next state and then just execute it.
