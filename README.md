# System T in Twelf

To run, start `twelf-server` and load `system-t.elf`.

```
$ twelf-server
Twelf 1.7.1 ...
%%% OK %%
loadFile system-t.elf
top
?- has-typ (lam nat [x] x) T.
Solving...
T = nat => nat.
```

You can evaluate things like this:

```
?- step (ap (lam nat [x] (s x)) (s s z)) E.
Solving...
E = s s s z.
```
