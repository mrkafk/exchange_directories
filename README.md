# exchange_directories

Change directories quickly, using e.g. first-letter abbreviation of entire path.

This is an OLD program, but it still works.

# I did not write this program, merely host it here because it no longer seems to be available in old repository.
# Actual author of the program is Frank B. Brokken.

See `xd.README` for more details.

# How it works

1. compile the program

`./build`

2. copy `xd` binary somewhere to your PATH.

3. add following function to your `.bash_profile`:

function cx ()
{
            cd `/usr/local/bin/xd \$*`
}

4. now, if you issue

`cx ulb`

you'll get multiple choice if "ulb" resolves to many paths on your system. Just press a char corresponding to path you want to go to:

```
% cx ulb
Multiple Solutions:
 1: /usr/lib/binfmt.d/
 2: /usr/local/bin/
```
On pressing `2` you're in `/usr/local/bin`.

