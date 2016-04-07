-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA512

# My GPG Public Keys

## Update - 2016-04-07

Changed the public key name to match the GPG Key ID (D89D82B4.asc) and updated
the verification instructions.

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

    git tag -v v2.1.0
    
You may need to fetch the tag from github first, but if all goes well you
should see something like this:

    object a93b188bbac2e73e40b34b6ab99d01120fae56ec
    type commit
    tag v2.1.0.pre
    tagger Ian D. Eccles <ian.eccles@apocryphilia.net> 1460045772 -0400

    Updated key and instructions
    gpg: Signature made Thu Apr  7 12:16:57 2016 EDT using RSA key ID 355EB117
    gpg: Good signature from "Ian D. Eccles <ian.eccles@apocryphilia.net>"
    gpg:                 aka "Ian D. Eccles <ian.eccles@gmail.com>"
    gpg:                 aka "Ian D. Eccles <whollychao@gmail.com>"
    gpg:                 aka "Ian D. Eccles <iande@mathish.com>"
    gpg:                 aka "Ian D. Eccles <ian@godel>"

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
Comment: GPGTools - https://gpgtools.org

iQIcBAEBCgAGBQJXBojqAAoJEOkRk6E1XrEX3B0P/0MCSw9237fDTxv3AJMvWfbc
Wi3td2/4NJsfpUkmUzQ0n8V4xJkikeElD40n9G5IOMtkj7ZMhXdsKJOhHRBynSKW
MYAq9cLCIm4eozKAYWm5RmWVj4T485MdQFhxwlolYNzP+LJBcefOm9g6j9TMu/zs
w/Ny9l2aRAB4+vt6auywltsqdiNwjb6AQ2peETNVlLNYFiWwOY9z/SeoFMdZlbYV
TW9v1Af8RoF5/2K+CdkPOQMRrRYGa5qW+wfqEdfqyPZq9S7C+2997HofSvOsqX7o
PAr8cmQepoXrGOg6bpgPfWJk/iExq3+ntJbqwOeIXvsZeivQn7hcVU/Ug69fW6kD
pslMuwt4Fic15r5ckolCF/wQmPh1KMsR+rgPDM0vv3zNiYT8BWaymtLYO6jI2eKd
8PylfRBWoB2KKSlbkgS2UX7c08gKNeztkqNLQ6PT0Kuo4xHNwhqOFFnUMP8jtU4C
pptjNtcX5ugiLN41cDK067eSuJMjtPNVR/g8WlojoqGEX9XTIeyLAstcfYRaSfyf
qH8kdMQ8kq76ZcqORDouxfJFCRLpZxWG4vdt18eVxL5RnOvHFF4XGQaq2JDAmMba
W7HXTCIgxPw91ZaS8h9D2H0cufpVTn56eS4Ez0katx8JHjs2ir9sRAXmWnEDSU5V
b6chzo7R0XrQRK/B3Cfc
=sFoV
-----END PGP SIGNATURE-----
