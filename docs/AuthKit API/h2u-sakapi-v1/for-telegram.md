# For Telegram

!!! info ""
    Currently, for Telegram, you can use **/AuthKit API** to send OTP codes to users via [**AVCBot**](https://t.me/AppVerifyCode_bot).

!!! warning ""
    * To obtain **Chat ID** for verifying Telegram users, you need to ask them to start [**AVCBot**](https://t.me/AppVerifyCode_bot) so that **/AuthKit** can identify the user according to [**Telegram's Official Documentation**](https://core.telegram.org/bots/#how-are-bots-different-from-users). Then, instruct them to retrieve the **Chat ID** from the message sent by **AVCBot** after they start the bot.
    * If you use this API on a Telegram dApp, you only need to ask users to start the bot, as their **Chat ID** is already provided to the application when they running the dApp.

!!swagger-http https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/AuthKit-API/openapi-specs/sak-telegram.json!!