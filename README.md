-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA1

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

iQIcBAEBAgAGBQJP6y0yAAoJEOkRk6E1XrEX+kwQAKeSIS+5pg1X5ZpTSRlUDSZR
x8lCb/rTAVLJKhjKIFmna6htevZacO94+K9JOy0oTOQefWVhRafGJQ+egfQ5ujlc
eDdR6B8noONL82yXElBFLZomUNhXKmSYzWBwT4XQzHSi5cWSO/ggzxGpdfSj/SOO
m6a/v1fvX81ydML2lXBN5++Ew0q2TDdFei3qUxLYRD22jMJ+9r33wUaHCq4Z5vPv
SU7dc9O7IPpV7NN7zpAaPHaYUfg6YoNHo4q7B4wHtgj5XjLhcNP1A1iTE3vVVDsv
/vLt5+8Onc3N8BUBoxwJiqJJMkotXzI41oEqbORXQl5ySs3SOX/kvGWLqCiSxmg2
PZq43xk+f+idzgEHllRj0tctykkN699MZBZpUy61gXBtT9jBjsCbFUB6oIboib8b
r1T0329qbDibjXqZAG7XqJE4hHrHMU+3bmUooeyRoqBVLZphlecv1ZPHWERjJ5Zb
4EEo/jYxG74PWQJoVzKgoStrjAxRz7x5PpZgY/K2xlMb0F16ZXnBz6DEGr7u9q2p
6/47MZ9s/0JkT/g2/dg8pfI8PRRu1AcUg0u4V7hxdqbZPoTMoaIEtOOf5DFfvqKf
ZpA5MqmdfxFhsowYsEACDS5jKCSqyWOyH4JYGrKHafM1RwJOVSwYByB85gdtAp0A
d/WNp/KqHVLmOuEBE5FQ
=jhUa
-----END PGP SIGNATURE-----
