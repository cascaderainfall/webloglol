---
Date: 2023-02-05
Type: Page
Tags: GrapheneOS, Google, Anonymity
---

# How to Create and Use a Google Account Anonymously on GrapheneOS

---

## Creating The Account
This part is not exclusive to [GrapheneOS](https://grapheneos.org) and can be done with any device but it's recommended to do it with GrapheneOS and that's what this guide covers.


There are essentially 3 ways to create a Google account anonymously
1. [**Public Wi-Fi**](#public-wi-fi)
2. [**Free VPN / Tor**](#free-vpn--tor)
3. [**Paid VPN**](#paid-vpn)

[**Anonymous Phone Verification**](#anonymous-phone-verification) can be used in combination with any other method for convenience or reducing trouble.

</br>

### Public Wi-Fi
Basically go outside, touch some grass; and find a place with public access free Wi-Fi. After connecting to the Wi-Fi, open a fresh incognito tab on Vanadium, go to `google.com` and create an account.
If you're lucky, Google won't ask for a phone number, and you're good to go!

I have used this method at coffee shops, restaurants and stores all over town and it has worked like a charm.  

</br>

### Free VPN / Tor
This method involves more luck than the others. Use any free VPN you want (or Tor) and hope you get an exit IP that isn't blacklisted by Google.
The procedure is:
1. activate VPN
2. open a fresh incognito tab in Vanadium
3. go to `google.com` and press sign in, then create account
4. try to create an account
5. if it says phone number required, fully exit out and close Vanadium from the task switcher
6. change VPN / Tor server and repeat

Note that using Tor will likely get your account flagged and Google to ask for phone number verification. See [Anonymous Phone Verification](#anonymous-phone-verification).  

</br>

### Paid VPN
This method involves using a paid VPN so that you can choose VPN servers that are unlikely to be blacklisted by Google. 

I myself create accounts using this method with Mullvad VPN and have not had much trouble. Heck, I created one just now!
<details>
  <summary style="color: #26b72b; padding: 2px 6px; width: 15em; border: solid; box-shadow: 3px 3px 4px black; cursor: pointer; background-color: #343434; list-style: none;"> click to load external image </summary>
  <img src="https://cascade.url.lol/wowthatwaseasygoogle" alt="Well that was easy! I swear this used to be harder lol" loading="lazy" style="border: dashed cyan;">
</details>

Servers in these countries have high success rates:
- Lithuania \[li]
- Luxembourg \[lu]
- Estonia \[ee]
- Romania \[ro]
- Switzerland \[ch]
- other Eastern European countries

The procedure is:
1. activate VPN
2. open a fresh incognito tab in Vanadium
3. go to `google.com` and press sign in, then create account
4. try to create an account
5. if it says phone number required, fully exit out and close Vanadium from the task switcher
6. change VPN server and repeat

</br>

### Anonymous Phone Verification
This is not an account creation method per se, but rather a way to create/secure an account with phone number verification without providing your real phone number. This allows you to create an account using any other method, even if Google forces you to enter a phone number. And it can be done WHILE or AFTER creating the account.

This method involves purchasing an SMS verification from a paid SMS verification website. Making the purchase anonymously (e.g. with Monero) is up to you. 

I've used this method with 5sim *-dot-* net and had problems after the initial account creation.

Note that this method is the safest for persistent (non-throwaway) accounts as Google is highly unlikely to flag your account or ask for a phone number later on. And it allows you to turn on Google's *account data deletion after inactivity* feature.

BTW, don't try free SMS verification sites as they don't work and are just a waste of your time.

</br>

## AFTER YOU SUCCESSFULLY CREATE THE ACCOUNT
Immediately go into your Google account settings and enable **2FA**. Make sure to save the backup codes, too. 
Turning on 2FA will greatly reduce the chance of your account getting flagged/banned and save you a lot of hassle. TOTP is recommended but FIDO2 will work just as well. Don't use SMS for 2FA. 

DO NOT SKIP THIS STEP NO MATTER WHAT METHOD(S) YOU USE

</br>
</br>

## Using The Anonymous Account on GrapheneOS
If you are going to use GrapheneOS's **sandboxed Play Services** there are a few things to keep in mind. You should create a new user profile and install a VPN / Orbot FIRST. To install, you can get the APKs from Aurora Store / GitHub or, if you already have Play Services on your 'Owner' profile, by cloning them. Depending on which VPN/Tor app you use.
Connect to your VPN/Tor and enable `Always on VPN` and `Block connections without VPN`. It is important from now on that you **DO NOT** use this profile with `Always on VPN` turned off.
Next, install the sandboxed Play Services apps from 'Apps' as you wish. Sign in to your new anonymously created account and you are good to go. (But not really)

However, this is not the end. You need to beware of bad practices that can deanonymize you.
It is **UNACCEPTABLE** to log in to this account on any profile which already has/had Play Services as every profile on Android has an app ID based unique identifier which can be used by Google or other parties to deanonymize you. See (grapheneos.org/faq#non-hardware-identifiers)[https://grapheneos.org/faq#non-hardware-identifiers]
If you have the exact same apps installed on a profile with another Google account logged in, Google can theoretically make a connection between the accounts.

Also, Play services can also read the country code of your SIM card when it is inserted into the device. For example, Google will know that a `+49` (Germany) SIM card is inserted but will not know the full number. I am not sure about eSIMs.
Play Services can also see how much global empty storage space is available on the device.

</br>

## General Advice
**DO NOT** use the Google account on your private (home/mobile) internet without a VPN/Tor. Google will associate your IP address to the accounts and you will lose your anonymity.

It is recommended to use the **Always on VPN** and **Block connections without VPN** features on GrapheneOS on profiles with this Google account. Note that Sandboxed Play Services is always active if it's enabled, so even disabling `Always on VPN` for a split second can deanonymize your account.

**DO NOT** use other names/pseudonyms you used on other Google accounts or anywhere really.

**DO NOT** log in to your other Google accounts on play services.

**DO NOT** make your account too similar to your other accounts.

**DO NOT** turn on `Google Location Accuracy`.

**DO** use common sense.

</br>

**Disclaimer**: I am in no way affiliated with any of the services/websites/products mentioned here.

</br>

Thanks to my friend Netcake for his help in research, testing, and writing.

</br>

##### Feedback
Contact me on Matrix (`@cascaderainfall:matrix.org`) or shoot me an email at `feedback -at- mail.cascade.omg.lol` or literally any other way listed on [my profile](https://cascade.profile.lol) for feedback and suggestions.
##### Want to improve this page?
Check out this blog's [GitHub repository](https://github.com/cascaderainfall/webloglol).

<div style="display:none;">
<video>
<source src="https://cascade.url.lol/anonymousgoogleaccountguide">
this is just an anonymous visitor counter (collects no data)
</video>
</div>