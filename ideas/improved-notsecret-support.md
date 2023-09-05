# Improved `notsecret` support

There are cases where it'd be nice to put comments in proximity to the value
instead of directly after it.

We want to make sure to not accidently ignore a real secret next to the
notsecret line

There could be some kind of restriction that it has to either be on the
line of the secret or on its own line above the line it's ignoring
or have some kind of notsecret+n syntax that allows ignoring n lines after
where `notsecret` == `notsecret+0` or something like that.

Maybe even support `notsecret-n` as well for places where it'd need to cover
the reverse. and notsecret+EOF for the whole file.

Anywho, just a placeholder for the idea and more discovery is needed.
