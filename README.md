# Dynamic voice-enabled keyboards

The DynamicKeyboard nodes combine DynamicKeyGrid and VoiceTextEditBox nodes to provide a single node that supports text entry in multiple languages and voice entry in English.

- The **DynamicKeyGrid** provides keyboard functionality. The layout of the keyboard is based on a JSON-formatted Key Definition File. 

  The classes derived from DynamicKeyboardBase (DynamicKeyboard, DynamicPinPad, and DynamicMiniKeyboard) have built-in Key Definition Files. For example, the DynamicKeyboard node uses a Key Definition File that matches the key layout of the [legacy Keyboard node](https://developer.roku.com/docs/references/scenegraph/dialog-nodes/dialog.md). 

  The **DynamicCustomKeyboard** node enables developers to define a custom Key Definition File in order to configure the key layout. In the Key Definition File, the developer specifies the keys in each section and row of the keyboard. The keys support the characters in the Basic Latin, Latin 1 Supplement, Latin Extended-A, and Latin Extended-B blocks. This provides support for most Western European languages, including English, French, German, Italian, Portuguese, and Spanish. 

- The **VoiceTextEditBox** displays the text that has been entered or spoken. This node supports multiple voice entry modes for entering email addresses, passwords, street addresses, and PINs. This node currently supports voice entry in English only.

> Developers should upgrade the [legacy keyboards](https://developer.roku.com/docs/references/scenegraph/dialog-nodes/dialog.md) in their channels to dynamic voice-enabled keyboards in order to leverage the following benefits: 
>
> - **Faster on-device sign-ups and sign-ins.** Enable customers to use voice entry to provide PIN codes when subscribing to channels and passwords when logging in. 
>
> - **Localized in-channel search**: Enable customers to search for content in their native language. 
>
> - **Localized customer information entry**: Enable customers to enter their personal information in their native language. 
