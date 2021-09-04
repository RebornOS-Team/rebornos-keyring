# rebornos-keyring

**Note from Rafael:**

keys located at: **/usr/share/pacman/keyrings/**

**rebornos-keyring** installs the authorized gpg keys from RebornOS

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/rebornos-special-system-files/rebornos-keyring.git
```

<br>

**rebornos-trusted** file explained:
```
2F6D8657D79199892002E6465F819C731E28BDAE:4: Rafael Costa Rega
0311C418E0EC1E68B69AA32A4833909AF8E40823:4: Azaiel (New)
2DD26266ABFEDBE49E7B7D330218E21BB4BC1E95:4: shivanandvp (new)
634862E57AB72263FB556DC92A54E5AA978177B3:4: Cookie Alice
38D3F838D6A0A3AB32DDDF2299EABCFB664B3E5F:4: SoulHarsh007
```

<br>

**How to get the value indicated above?**

Once we have the gpg key created in our system, it will be enough to execute the following from the terminal:

```
$ gpg --list-secret-keys --keyid-format LONG
/home/user/.gnupg/pubring.kbx
-----------------------------
sec   rsa4096/xxxxxxxxxxxxxxxxxxx 2019-09-05 [SC]
      xxxxxxxxxxxxxxxxxxxxxxxxxxx --> **Send me this number**
uid   ....
ssb   rsa4096/xxxxxxxxxxxxxxxxxxxx
```


Send me the number marked by -->****Send me this number****  and also send me your **gpg public key**.

Your public gpg key must be in the file **rebornos.gpg** (the format is clearly visible when accessing that file).

How do you send your public pgp key to a file? From the terminal, it is done with:

```
gpg --armor --export >> your_name_for_example.asc
```

Please, send me this file.

Checking what is needed: it is the file with your **public pgp key**, and the value indicated above.


<br>

**You can read about the procedure to create a pgp key here:**

https://www.inmotionhosting.com/support/edu/everything-email/how-to-create-a-gpg-key/


Content of the file **rebornos-revoked**

```
C4582C50B616BCEA9078B47D6ACC7316B56B3157 Azaiel old key
916455D2C5A3F27F2280A5AC55D64E0D48DE87B0 Shivana old key
428836525A2B0D53B8F97ABDDBF573D69DE9F4B5 Keegan Milsten (Old)
DB1CC7C341382E070279E7DAA68B7FA972447061 Keegan Milsten (new)
```
<br><br>
This corresponds to Azaiel's old pgp key. Since it was never used, it is revoked:

**C4582C50B616BCEA9078B47D6ACC7316B56B3157:4: Azaiel (Old)** --> Revoked.

<br><br>
This corresponds to Shiva's old pgp key. Since it was never used, it is revoked:

**916455D2C5A3F27F2280A5AC55D64E0D48DE87B0 Shivana (Old)** --> Revoked.

<br><br>
This corresponds to Keegan Milsten (Old) pgp key (revoked):

**428836525A2B0D53B8F97ABDDBF573D69DE9F4B5**

<br><br>
This corresponds to Keegan Milsten (new) pgp key (revoked):

**DB1CC7C341382E070279E7DAA68B7FA972447061**
<br><br>
**End note from Rafael**
