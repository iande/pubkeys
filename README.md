# My GPG Public Keys

## ian.eccles@gmail.com.asc

As the name suggests, I use this key for signing/decrypting emails.  I also
use it to sign tags in my public git repositories.

## ian@godel.asc

This guy tends to get used on my laptop and doesn't tend to venture out
into the public eye on its own.  I only include it here because I sign my
other keys with it.

## Verifying

Verifying `ian.eccles@gmail.com.asc` should require nothing more than a GPG
suite and this repo.  Import the key, then verify tag `gmail` of this repository:

    git tag -v gmail
    
You may need to fetch the tag from github first, but if all goes well you
should see something like this:

    object cbc83dc3090c6e197ac4490d67812252c85ef3b6
    type commit
    tag 1.0
    tagger Ian D. Eccles <ian.eccles@gmail.com> 1299202449 -0500

    seems like a reasonable thing to do
    gpg: Signature made Thu Mar  3 20:34:10 2011 EST using RSA key ID F7278153
    gpg: Good signature from "Ian D. Eccles <ian.eccles@gmail.com>"
    gpg:                 aka "Ian Eccles <ian.eccles@gmail.com>"


Similarly, for `ian@godel.asc`, you can verify it against the `godel` tag.

    git tag -v godel


It occurred to me after starting this repo that these public keys have my
screaming head avatar embedded in them.  So, that should explain why each
key is roughly 9Kb larger than it need be.
