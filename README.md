# omerta: code of silence

This project is developed during the ETHBerlinZwei hackathon (2019).

*Omertà is a Southern Italian code of silence and code of honor that places importance on silence in the face of questioning by authorities or outsiders; non-cooperation with authorities, the government, or outsiders; [wikipedia](https://en.wikipedia.org/wiki/Omert%C3%A0)*

##  Let's use Facebook, but with end-to-end encryption! 

This is not a troll, people use Twitter and Facebook and it is not ready to change. People have their habits and above all, their friends and their network are on it and that create a significant retention of users.

Finally, in an ideal world we could continue to use our favorite social networks by adding a feature that would give me a real control of my data.

Starting from this idea, we imagined a solution as transparent as possible for users of these social networks through the use of a browser extension.

Bob and Alice are friends on Facebook.
They install the Chrome browser extension "Omerta" and initialize it with their Ethereum account with enough Eth to make only 1 transaction on the mainnet.
And that's all.

Lorque Bob instal the extension, he create his mafia by filling the public keys of the member of his mafia (this step could be automated by allowing a Facebook app Omerta that would access the open graph api, we decided not to focus us on this part during the Hackathon)

How to make sure that only Alice can decode Bob's messages? (and not Mark)
Bob generates a secret locally, he encrypts it with Alice's public key, then sends a transaction to Alice with the encrypted secret in the data field of the transaction.

Thanks to the browser extension, when Bob posts a new status on Facebook, Omerta encrypts the message before sending it to Facebook's Backend.

When Alice loads her Facebook wallet with all the statuses of her friends, Bob's encrypted status is decoded and replaced on the fly in HTML by the Omerta extension.

With this system, Bob and Alice have all the advantages of Facebook without the disadvantages.

From Facebook's point of view, this hijacking is not easy to detect and sensure, and techniques of offustation can always be added to Omerta to get a head start.


## What is Omerta?
![omerta](https://github.com/vincentlg/omerta/blob/master/berlin-hack-1.png)
