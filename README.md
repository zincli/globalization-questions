# Questions About Globalization

## i18n

### Messages(or Copy?) Management

How do you manage application's messages? A system for creating & translating?

### Working Flow

What is the best practice of i18n development?

For example, we have same messages in all App of iOS, Android & Web(mobile & desktop).

* Should we use same message IDs for all of them?
* Which role is the one should responsible for creating the message ID?
* How to make the development concurrent?
* How to get the translators know the context of messages?


## L10n

* How to get translators handle the plural rules of ICU Message Format?
* Client side formatting or server side formatting?
  * Client side formatting has many problems
      * ICU tool for iOS and Android is dependent on OS version or need extra plugin.
      * Web's Intl(ECMA402) also dependent on browsers' implementation. 
          * Browser's implementation have bugs as using old version of CLDR, and not easy to upgrade.
          * Polyfills' size is too big.