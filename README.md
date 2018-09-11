# easyCA

# Coming soon!

After needing to deploy a private certificate hierarchy for a small project, I discovered that there were three ways to do it:

* Download and deploy some pre-baked VM image of some complex rocket ship, where you have no friggin idea if the creator left in something sneaky and half the clickie-buttons might as well be in a foreign language
* Spend a few days going through the mental gymnastics to buold the above spaceship yourself
* Follow some sketchy guide posted on a random blog somewhere that's hard to follow because can not people if maybe use proper grammer

To that end, I'm building out a pile of bash scripts that can do the heavy-lifting for you. The idea:

1. Start with a vanilla Ubuntu server ISO (Hash check it against Canonical's md5sums if you have an affection for tin foil)
2. Toss that ISO on a VM or a junkbox that's about to die anyway and install Ubuntu
3. git clone this script onto that Ubuntu VM / dustbin 
4. Install the openssl package (Available on the ISO'd built-in repository so you can keep poor Edsol airgapped from the horrors of the Internet)
4. Run the script
5. Download the certificates onto a flash drive labeled "Sword of a Thousand Truths" / floppy disk labeled "NetBEUI drivers". You can even print it out on your dot matrix or even use smoke signals if you want.
6. When done, throw away the keys for the root CA. Or the entire virtual machine. Or the entire computer. Whichever works for you and your compliance regime.

The idea is nothing sneaky is going on, and you can be assured of that because the only thing that's not yours is the few hundred lines of code that you can look over anyway (FYI - I'm a crappy programmer so please be gentle)

PS. Name likely to change as I'm too lazy to do a trademark check, so if this gets downloaded by somebody other than me and my grandma I may change the name before some lawyers send me a nastygram.
