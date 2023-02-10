---
Date: 2023-02-05
Type: Page
Tags: GrapheneOS, Google, Anonymity
---

# How to Create and Use a Google Account Anonymously on GrapheneOS

---

## Creating The Account
This part is not exclusive to [GrapheneOS](https://grapheneos.org) and can be done with any device but it's recommended to do it with GrapheneOS and that's what this guide covers.


There are essentially 3 ways you can create a Google account anonymously
1. [**Public Wi-Fi**](#public-wi-fi)
2. [**Free VPN / Tor**](#free-vpn--tor)
3. [**Paid VPN**](#paid-vpn)

[**Anonymous SIM verification**](#anonymous-sim-verification) can be used in combination with any other method for convenience or reducing trouble.

</br>

### Public Wi-Fi
Basically go outside, touch some grass; and find a place with public access free Wi-Fi. After connecting to the Wi-Fi, open an incognito tab on Vanadium and go to `google.com` and create an account.
If you're lucky, Google won't ask for a phone number, and you will be good to go!

I have used this method with coffee shops, restaurants and shops all over town and it worked like a charm.  

</br>

### Free VPN / Tor
This method involves more luck than the others. Use any free VPN you want (or Tor) and hope you get an exit IP that isn't blacklisted by Google.
The procedure is:
1. activate VPN
2. open incognito tab in Vanadium
3. go to `google.com` and press sign in, then create account
4. try to create an account
5. if it says phone number required, fully exit out and close Vanadium from the task switcher
6. change VPN / Tor server and repeat

Do note that using Tor is likely to get your account flagged and Google to ask for phone verification. See [Anonymous SIM verification](#anonymous-sim-verification).  

</br>

### Paid VPN
This method involves using a paid VPN so that you can choose VPN servers which are likely not blacklisted by Google. 

I myself create accounts using this method with Mullvad VPN and have not had much trouble. Heck, I created one just now!<sup>[\[external image\]](https://cascade.url.lol/wowthatwaseasygoogle)</sup>

Servers in these countries have high success rates:
- Lithuania \[li]
- Luxembourg \[lu]
- Estonia \[ee]
- Romania \[ro]
- Switzerland \[ch]
- other eastern European countries

The procedure is:
1. activate VPN
2. open incognito tab in Vanadium
3. go to `google.com` and press sign in, then create account
4. try to create an account
5. if it says phone number required, fully exit out and close Vanadium from the task switcher
6. change VPN server and repeat

</br>

### Anonymous SIM verification
This is not an account creation method by itself but rather a way to create/secure an account with phone verification without giving your real phone number. By doing this, you can create an account with any other method, even if Google forces you to give a phone number. And it can be done WHILE or AFTER creating the account.

This method involves buying an SMS verification on a paid SMS verification website. Making the purchase anonymously (e.g. with Monero) is up to you. 

I've used this method with 5sim *-dot-* net and had no trouble after the initial account creation.

Do note that this method is the safest for persistent (non-throwaway) accounts as Google is highly unlikely to flag your account or ask for a phone number later on. And it allows you to turn on Google's *account data deletion after inactivity* feature.

BTW, don't try any free SMS verification sites as they will not work and cause you to waste time.

</br>

## AFTER YOU SUCCESSFULLY CREATE THE ACCOUNT
Immediately go into your Google account settings and turn on **2FA**. Make sure to save the backup codes as well. 
Turning on 2FA will greatly decrease the chance of your account getting flagged/banned and save you a lot of trouble. TOTP is recommended but FIDO2 will also work fine. Don't use SMS for 2FA. 

DO NOT SKIP THIS STEP NO MATTER WHAT METHOD(S) YOU USE

</br>
</br>

## Using The Anonymous Account on GrapheneOS
If you will be using GrapheneOS's **sandboxed Play Services** there are a couple of things to keep in mind. You should create a new user profile and install a VPN / Orbot FIRST. To install, you can get the APKs from Aurora Store / GitHub or, if you already have play services on your 'Owner' profile, by cloning them. Depending on which VPN/Tor app you use.
Connect to your VPN/Tor and turn on  `Always on VPN`  and  `Block connections without VPN` . It is important from now on that you **DO NOT** use this profile with  `Always on VPN`  turned off.
Next, install the sandboxed Play Services apps from 'Apps' as you wish. Sign in to your new anonymously created account and you are good to go.

However, this is not the end. You need to beware of bad practices that can deanonymize you.
It is **UNACCEPTABLE** to log in to this account on any profile which already has/had Play Services as every profile on Android has an app ID based unique identifier which can be used by Google to deanonymize you.
If you have the exact same apps installed on a profile with another Google account logged in, Google can theoretically make a connection between the accounts.

Also, Play Services can read your SIM's country code if the SIM card is in the device. For example, Google will know a `+49` (Germany) SIM card is inserted but will not know the full number. I am not sure about eSIMs.
Play Services can also see how much global empty storage space there is on the device.

</br>

## General Advice
**DO NOT** use the Google account on your private (home/mobile) internet without a VPN/Tor. Google will tie your IP address to the accounts and you will lose your anonymity.

It is recommended to use the **Always on VPN** and **Block connections without VPN** features on GrapheneOS on profiles with this Google account. Note that Sandboxed Play Services is always active if it's enabled, so even disabling  `Always on VPN`  for a split second can get your account deanonymized.

**DO NOT** use other names/pseudonyms you used on other Google accounts or anywhere really.

**DO NOT** log in to your other Google accounts on play services.

**DO NOT** make your account too similar to your other accounts.

**DO NOT** turn on  `Google Location Accuracy`.

**DO** use common sense.

</br>

**Disclaimer**: I am not affiliated with or tied to any services/websites/products mentioned here in any way.

</br>

Thanks to my friend Netcake for his help in research, testing, and writing.

</br>

##### Feedback
Contact me on Matrix (`@cascaderainfall:matrix.org`) or shoot me an email at  `feedback -at- mail.cascade.omg.lol` 
 or literally any other way listed on [my profile](https://cascade.profile.lol) for feedback and suggestions.
##### Want to improve this page?
Check out this blog's [GitHub repository](https://github.com/cascaderainfall/webloglol).

<div style="display:none;">
<video>
<source src="https://cascade.url.lol/anonymousgoogleaccountguide">
this is just an anonymous visitor counter (collects no data)
</video>
</div>