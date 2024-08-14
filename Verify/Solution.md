# Verify_FORENSICS

Verify was the first challenge i solved, it is part of the _FORENSICS_
chanlenges.

### Description

> People keep trying to trick my players with imitation flags. I want to make
> sure they get the real thing! I'm going to provide the SHA-256 hash and a
> decrypt script to help you know that my flags are legitimate.

From the challenge description, we see a couple of keywords, that were new to
me;

- SHA-256 hash
- decrypt script

Upon starting the instance, you'll be able to download a couple of files and a
folder with a bunch of files with random names.

The goal of the challenge is to use the SHA-256 hashing function to check which
file is legitimate, hence containing the real flag.

NOTE: When i first heard of SHA-256, i thought it was an encryption method used
to protect sensitive data, so that data can be decrypted later and use - > I was
half right.

## SHA-256 ???

SHA-256 is what's referred to as a hashing function; hashing is a one-way
process,meaning you cannot reverse the process to obtain the original input from
the hash.

_The primary use of hashing is to verify data integrity and store passwords
securely_

I suggest playing around with the `sha256sum` command if you're on linux or mac.

In our case we do have the hash, and just need to check which file in our "files
folder" is the real thing; to do that we can either create a script to go
through all files or do what i did as a beginner:

RUN

```bash
sha256sum *
```
