# Orion Translations Guide

Orion applications must be internationalized to support the following languages and locales.

* German - `de`
* English - `en`
* English (Australia) - `en-AU`
* English (Canada) - `en-CA`
* English (United Kingdom) - `en-GB`
* English (United States) - `en-US`
* Spanish - `es`
* French - `fr`
* Dutch - `nl`
* Dutch (Belgium) - `nl-BE`
* Portuguese - `pt`
* Swedish - `sv`
* Swedish (Sweden) - `sv-SE`


Strings such as text, symbols, and date formats must be translated in all of these languages and locales. This guide covers the steps to translate the strings in your application.

1. Log a request to the [TRANS](https://jira.cerner.com/projects/TRANS/issues) JIRA project.
2. Select the desired languages for translation in the `Target Languages` field. The translation of text is expected to be identical across locales for a given language. However, symbols and date formats may differ between locales of the same language so it is important to call out in the TRANS JIRA the need to translate any symbols or date formats for each of the locale.
3. Attach the English translation file that contains all the keys and strings. Typically this is the `en.json` file in the `translations` folder.
4. When possible, attach screenshots capturing where each of the English strings are displayed in your application. The screenshots provide context for the translator to show where or how these strings are used so the strings are correctly translated with context. Without screenshots the translated strings could be out of context and lead to different meanings. The preferred way to provide these screenshots is to use the test evidence from the WDIO runs for the `en-US` locale since these should cover the entire workflow. 
5. After you receive all the translations update the translation files in your application. Capture screenshots in each of the languages showing the new translations. Add all the screenshots to the TRANS JIRA and ask the translator to validate that the translations look correct.
