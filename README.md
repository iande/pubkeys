-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA256

# My GPG Public Keys

## Update - 2012-06-27

I'm still fairly new to GPG, and like a tool I created a separate key-pair for
each different email address, rather than adding UIDs to an existing pair.
As a result of that and a desire to use key lengths of 4096 bits, I have
revoked my existing keys, and created a new one. This repository, and the
verification instructions, have been updated accordingly. The key size is also
smaller as I have not included my floating head photo this time.

If you have previously imported my old keys, you can feel free to remove them.
Updating them from your preferred GPG/PGP key server should result in them
being revoked, but I really haven't tested that. I have only verified that
key servers are reporting those public keys as revoked.

## Pubkey: ian.eccles@gmail.com.asc

This is my primary key-pair and includes a few additional UIDs for other
email addresses I have been known to use.

## Verifying

Verifying `ian.eccles@gmail.com.asc` should require nothing more than a GPG
suite and this repo.  Import the key, then verify tag `v2.0.0` of this repository:

    git tag -v v2.0.0
    
You may need to fetch the tag from github first, but if all goes well you
should see something like this:

    object 9efefadad5baacb99a530e7350ec446c2d16da46
    type commit
    tag v2.0.0.pre
    tagger Ian D. Eccles <ian.eccles@gmail.com> 1340809612 -0400

    tagged for example output
    gpg: Signature made Wed Jun 27 11:06:52 2012 EDT using RSA key ID 355EB117
    gpg: Good signature from "Ian D. Eccles <ian.eccles@gmail.com>"
    gpg:                 aka "Ian D. Eccles <whollychao@gmail.com>"
    gpg:                 aka "Ian D. Eccles <iande@mathish.com>"
    gpg:                 aka "Ian D. Eccles <ian@godel>"
    gpg:                 aka "Ian D. Eccles <Ian.Eccles@univwell.com>"

Your results will differ as this output is for a test tag I created for
demonstration purposes.

## Dead Keys

### Revoked

Below is a listing of the GPG keys which I recently revoked. These guys can
still be retrieved from various key servers, but I suspect most GPG clients
will provide a clear indication that the keys have been revoked. There are
a few others I revoked, but they were not previously associated with this repo.

    pub   2048R/0ABADE36 2011-02-08 [revoked: 2012-01-12]
    uid                  Ian Eccles <ian@godel>
    uid                  [jpeg image of size 9871]

    pub   2048R/F7278153 2010-03-02 [revoked: 2012-01-12]
    uid                  Ian D. Eccles <ian.eccles@gmail.com>
    uid                  Ian Eccles <ian.eccles@gmail.com>
    uid                  [jpeg image of size 9871]


### Lost Keys

Depending your GPG client and the key server you use, you may come
across two other 1024 bit DSA keys for `ian.eccles@gmail.com`:

    pub   1024D/75760FB0 2006-08-10 [expired: 2007-08-10]
    uid                  Ian Eccles <ian.eccles@gmail.com>

    pub   1024D/5AD26872 2005-10-13
    uid                  Ian Eccles <ian@mathish.com>
    uid                  Ian Eccles <ian.eccles@gmail.com>
    sub   2048g/3DD15C64 2005-10-13
    
Fortunately, I did set an expiration date on 75760FB0, so it's obviously
no good. However, 5AD26872 is forever lost.


## Signature

And just for kicks, I clearsign'd this file.



-----BEGIN PGP SIGNATURE-----
Version: GnuPG/MacGPG2 v2.0.17 (Darwin)
Comment: GPGTools - http://gpgtools.org

iQIcBAEBCAAGBQJP6y9rAAoJEOkRk6E1XrEXctYP/RlyszWdLtgd1vPcgLbLqTgw
X8sGaZ57Q3SD4/uA3LDoaQcP8ZrHDc5Dvl5PvtxH2JCrUvYJ8kIsDQow0kTGa4ZP
cG4LjtaWbj40Jc6SdiOBiBGIGxFErLxr5a8YgDOY9O/wCJg7D98pKsNVoi6c1Dy3
K5MizbWm5X/ZgjyxBBj1SMKo1RPP9ex1f4jITeehSupoV0CIPxjEE1+w2V6VPffl
W8RD89mwcDwmPQqmElXmSAgRi73uo9ExgF1n6JS/IGwLY8kOlqhWlyQvqvwQwvD9
rV+TMcPIKp2Yclcpllo3Q8GiwzLwZPmMWyd5kCOPjUdNHaPgdPOH3bJLvS6D1IvG
TlgKj2xG22Vm7P8OFld8jpctUs2y4wg2irikrVnQ3KZAQziLh4Ide7bHriyjXg7L
ap0rPMln21hNAIzRZ0RZ6pidj9vu4M5rVSBPZ3b18AohuPyqBSbzILHGZZMT7qX/
aXGqb0DQWz/oiC9YjBgNT68t4VPBssf9YnmYn8pWz1bsJ69ZzvGNRUAco/LVEq0R
N1yLmptfOgiKwNVTe3pI4uqQiafJgNTqgnrHGSYMCg8dp3A7fWiIajHTE5Q2tIV6
M17kgOSQcwwxi52Talt0kxU1tO07H2NLgQKXyyXACizjBhFxRF8F5QtwIaR3DrVM
oPKN1b+Fskk/fkM3pRvU
=2eVp
-----END PGP SIGNATURE-----
