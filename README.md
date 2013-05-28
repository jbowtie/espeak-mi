Espeak Māori data files
=======================

Māori voice definition for use with the espeak speech synthesis engine.

This project defines a Māori speaker. The current version simple adds Maori
language support, using the default phoneme tables included with the espeak program.

Future versions will refine the model and add a native speaker phoneme database.

Installing
----------

You will need to copy or symlink the `voices/mi` file to the espeak voices directory.
On my copy of Ubuntu, that location is `/usr/lib/x86_64-linux-gnu/espeak-data/voices`.

Once the voice file is in place, you can compile the dictionary using the `espeak compile=mi` command. If you get the error `Error in mi_rules, no default rule group` you are running an older version of espeak and can safely ignore it.

Usage
-----

See the [espeak documentation][1]. You can easily test it at the command line.

```
espeak -vmi "Kia ora."

espeak -vmi "He moana pukepuke e ekengia e te waka."
```

[1]: http://espeak.sourceforge.net/index.html
