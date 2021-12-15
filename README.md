# ColdCard Ultra Quick Guide
An ultra quick guide for beginners to get you from zero to self-custodied cold storage in as few steps as possible. 

<p align="center">
  <img width="756" height="441" src="Assets/UltraQuickTitleImage-M.png">
</p>

This guide covers:
- Checking the tamper-evident bag
- Setting up a PIN
- Generating a seed phrase
- Connecting ColdCard to [Sparrow Wallet](https://www.sparrowwallet.com/)

## Checking the tamper-evident bag:
Upon receiving your ColdCard, ensure that the tamper-evident bag has not been compromised. If anything seems amiss or if you have any problems contact [support@coinkite.com.](mailto:support@coinkite.com?subject=%5BContact%5D%20-%20) Visually inspect the surfaces and edges of the bag for indications of tampering, openings, or damage.

<p align="center">
  <img width="400" height="300" src="Assets/Bag0.png">
  <img width="400" height="300" src="Assets/Bag1.png">
</p>

<p align="center">
  <img width="400" height="300" src="Assets/Bag2.png">
  <img width="400" height="300" src="Assets/Bag3.png">
</p>

You will see the tamper-evident words "void" appear when the seal is opened. Inside you will find your new ColdCard, the Wallet Recovery Backup Card, sticker(s), and an additional copy of the bag number which should match the bag number printed on the outside of the bag. 

<p align="center">
  <img width="388" height="208" src="Assets/IMG_6079.JPG">
  <img width="399" height="277" src="Assets/IMG_6080.JPG">
</p>

If everything looks good, then you are ready to power on your new ColdCard and get it setup. 

## Setting up a PIN
Here is a diagram you can reference to learn the ColdCard's navigation:

<p align="center">
  <img width="853" height="505" src="Assets/Navigation.png">
</p>

To power on the ColdCard simply connect a USB to micro-USB [cable](https://store.coinkite.com/store/category/accessories) to the port on top pof the ColdCard and the other end to a USB port on your computer. Keep in mind, if you want to keep your ColdCard air-gapped then the [Middle Ground](https://www.github.com/econoalchemist/ColdCard-MiddleGround/) guide may be more appropriate for you, this guide will demonstrate how to use ColdCard connected to a computer.

First, read and accept the terms of sale & use. Then you will be asked to confirm the bag number. If there are any discrepancies, contact [support@coinkite.com](mailto:support@coinkite.com?subject=%5BContact%5D%20-%20).

<p align="center">
  <img width="605" height="454" src="Assets/BagNumber.jpg">
</p>

Make careful considerations with your PIN number. You don't want to use one that is easy to guess. Your PIN will have two parts, a prefix and suffix. The idea is that once you enter the prefix, you will be presented with two anti-phishing words. If the words are the same as the words that were originally presented to you at initial startup, then you know that your ColdCard has not been tampered with since the last time you accessed it. 


First, select "Choose PIN Code", then you will see a brief description of how the PIN code works. Each part of your PIN code can be between 2 and 6 digits. There is absolutely no way to access a forgotten or lost PIN. And if you enter a PIN incorrectly too many times, it will brick your ColdCard as a security feature.

<p align="center">
  <img width="605" height="454" src="Assets/Choose PIN.jpg">
</p>

After hitting "OK" you will get one more warning about the risk of losing or forgetting your PIN. After reading that, you can enter your PIN prefix. Use the included notecard to write down your PIN prefix then hit "OK". 

<p align="center">
  <img width="454" height="341" src="Assets/EnterPreFix.jpg">
  <img width="454" height="341" src="Assets/EnterPreFix2.jpg">
</p>

Next you will be presented with your two anti-phishing words. Write these down on your notecard.

<p align="center">
  <img width="605" height="454" src="Assets/AntiPhishingWords.jpg">
</p>

Next, enter your PIN suffix, then write it down on the notecard and hit "OK".

<p align="center">
  <img width="454" height="341" src="Assets/EnterSuffix.jpg">
  <img width="454" height="341" src="Assets/EnterSuffix2.jpg">
</p>

Then you will be asked to re-enter your PIN prefix, confirm the two anti-phishing words, and enter your PIN suffix. The ColdCard will save that information and then open up the wallet where you can generate your seed phrase.

## Generating a seed phrase
There are a couple considerations you may want to make when creating a seed phrase. For example, ColdCard will generate a seed phrase for you by default, as shown in this guide. However, maybe you don't trust the True Random Number Generator (TRNG) in your ColdCard, you can introduce your own randomness as shown in the [Middle Ground](https://www.github.com/econoalchemist/ColdCard-MiddleGround/) guide.

First, Select "New Wallet" and after a moment you will be presented with 24 words. Write these words down on your notecard. Then double check your work.
<p align="center">
  <img width="302" height="227" src="Assets/NewWallet.jpg">
  <img width="302" height="227" src="Assets/SaveWords1.jpg">
  <img width="302" height="227" src="Assets/SaveWords2.jpg">
</p>

Next, you will be tested on your seed words to ensure you wrote them down correctly. After passing the test, you will be in the ColdCard main menu. Make sure you store your notecard securely. Anyone who gains access to your seed phrase will be able to steal your bitcoin. Never share your seed phrase with anyone.

<p align="center">
  <img width="605" height="454" src="Assets/Test.jpg">
</p>

## Connecting ColdCard to Sparrow Wallet
Sparrow Wallet is a Bitcoin wallet designed to be connected with your own node and ran from your desktop computer. This is a user-friendly wallet with an intuitive interface and many advanced features for a range of capabilities. To learn more about Sparrow Wallet and for installation instructions, visit the [Sparrow Wallet website](https://www.sparrowwallet.com/).

In this guide you will see how to connect your ColdCard to Sparrow Wallet using a reputable public Electrum server as the backend. 

Once you install Sparrow Wallet and launch the application, you will be presented with an empty user interface. Navigate to "File>Preferences".

<p align="center">
  <img width="814" height="611" src="Assets/Sparrow0.png">
</p>

Then click on the "Server" tab on the left-hand side. Select "Public Server" at the top, choose a public server from the drop down menu, then click on "Test Connection". It should only take a moment for a sucessful connection to be made. You may have to try a couple different public servers to get a good connection. 

<p align="center">
  <img width="452" height="339" src="Assets/Sparrow1.png">
  <img width="452" height="339" src="Assets/Sparrow2.png">
</p>

Keep in mind that with this configuration, you are using a public Electrum server which means that your transactions will broadcast to a public server. Your bitcoin is not at risk but this method has a privacy tradeoff that is worth considering. In the [Middle Ground](https://www.github.com/econoalchemist/ColdCard-MiddleGround/) guide, I cover more privacy-focused options. To learn more about Sparrow Wallet best practices, check out [this](https://www.sparrowwallet.com/docs/best-practices.html) guide. 

You will notice in the Sparrow Wallet interface lower right-hand corner that the color has changed to yellow. This indicates that your wallet is using a public Electrum server as the back end. 

You can create your new wallet by selecting "File>New Wallet", then you will be asked to name this wallet. Name the wallet whatever you want then click on "Create Wallet". 

<p align="center">
  <img width="814" height="611" src="Assets/Sparrow3.png">
</p>

You will see the following screen, you can leave all the settings on the defaults. Plug your ColdCard into the desktop and log into it if you haven't done so already before clicking on the "Connected Hardware Wallet" button.

<p align="center">
  <img width="814" height="611" src="Assets/Sparrow4.png">
</p>

After you click on "Connected Hardware Wallet", a screen will pop up and you can click on the "Scan..." button. Then after a moment you should see ColdCard appear on screen with an "Import KeyStore" button, click on that button. 

<p align="center">
  <img width="452" height="339" src="Assets/Sparrow5.png">
  <img width="452" height="339" src="Assets/Sparrow6.png">
</p>

After a moment, you will see a summary of the wallet you are about to apply. You will notice a "Master fingerprint" dialog box with 8 charactersin it. You can use this unique identifier to confirm that you are importing the correct wallet from your ColdCard. On your ColdCard, from the main menu, navigate down to "Advanced>View Identity" and you can compare the displayed fingerprint to the one displayed in Sparrow Wallet. If everything looks good, then click on "Apply" in Sparrow Wallet. 

<p align="center">
  <img width="814" height="611" src="Assets/Sparrow7.png">
  <img width="814" height="350" src="Assets/Sparrow8.png">
</p>

After clicking on "Apply", you will have the opportunity to add a password to your wallet. This is a password which will encrypt the Sparrow Wallet data file that is saved on your computer. This password can protect your wallet if someone else gains access to your Sparrow Wallet file. If you forget your password, you will need to create a new wallet file by repeating this whole process. 

<p align="center">
  <img width="814" height="611" src="Assets/Sparrow9.png">
</p>

Now you can click on the "Receive" tab on the left-hand side of the Sparrow Wallet interface. Then you will be presented with a bitcoin receiving address, a QR code, and some additional details. You can scan this QR code with your mobile Bitcoin wallet, for example, and deposit some bitcoin to your ColdCard. You should see the transaction show up in Sparrow Wallet after a moment. The transaction will remain in a pending status until it receives some blockchain confirmations. In the mean-time, you can click on the "Transactions" tab and review further details about your transaction. You can also copy/paste your transaction ID in [mempool.space](https://mempool.space/) to watch for your first confirmation. 

<p align="center">
  <img width="452" height="339" src="Assets/Sparrow10.png">
  <img width="452" height="339" src="Assets/Sparrow11.png">
  </p>
  
  <p align="center">
  <img width="452" height="339" src="Assets/Sparrow12.png">
  <img width="452" height="219" src="Assets/Sparrow13.png">
</p>

You can disconnect your ColdCard from the computer and when you open the wallet in Sparrow Wallet in the future, several addresses will be saved so you can continue depositing to your ColdCard without having to re-connect it every time. It is best practice to confirm each receiving address on the ColdCard itself and also to only use address once. 

When you are ready to spend bitcoin from your ColdCard, navigate to the "Spend" tab on the left-hand side in Sparrow Wallet. There, you can paste the address you are sending to, add a label, enter an amount to send, and choose a miners fee rate, etc. Once you have everything set, click on "Create Transaction". On the next screen click on "Finalize Transaction for signing". 

<p align="center">
  <img width="452" height="339" src="Assets/Sparrow14.png">
  <img width="452" height="339" src="Assets/Sparrow15.png">
  </p>
  
Next you will asked to sign the transaction using your ColdCard. You can deposit bitcoin with your ColdCard disconnected but to spend bitcoin, the ColdCard needs to sign the transaction. Sparrow Wallet is used to build the transaction based on your deposits and the information you entered. Connect your ColdCard to your computer and log into it, then in Sparrow Wallet click on the "Sign" button. A pop up window will display your the option for ColdCard, click on the "Sign" button.

<p align="center">
  <img width="452" height="339" src="Assets/Sparrow16.png">
  <img width="452" height="339" src="Assets/Sparrow17.png">
  </p>
 
A moment later on the ColdCard, it will ask you to confirm. Hit the "Ok" button (Check Mark) and the ColdCard will sign the transaction and pass the details back to Sparrow Wallet. Then in Sparrow Wallet, click on the "Broadcast Transaction" button to send the signed transaction to teh Bitcoin Network. 

  <p align="center">
  <img width="452" height="339" src="Assets/Sparrow18.png">
  <img width="452" height="339" src="Assets/Sparrow19.png">
  </p>
