# Changelog

!!! info ""
    **/AuthKit API v2** has not been released yet. The expected launch date is Dec**ember 12, 2025**. You can experience its Beta version when a new announcement is made.

!!! success "NEW"
    [Use **`X.509`** certificates in **/AuthKit API v2**](#user-content-fn-1)[^1]

    * Public **`X.509`** Certificate ([`.avc-pubcert`](#user-content-fn-2)[^2]): Used to authenticate API request actions.
    * Private **`X.509`** Certificate ([`.avc-privcert`](#user-content-fn-3)[^3]): Used to manage applications on **AVCManager**.

!!! success "NEW"
    Some API endpoints will be added

    * `/api/tg/captcha`: Captcha verification via **AVCBot.**
    * `/api/url/tg` : Verify Telegram users by using a redirect URL to **AVCBot** and confirming their identity.
    * `/api/url/email`: Verify whether that email belongs to the person by requesting them to access the confirmation URL in the email.

!!! success "NEW"
    : Use an additional MySQL Database server as the second server.

!!! success "NEW"
    : New module created to make it easier to use **/AuthKit API v2** for **Python**.

!!! warning "CHANGE"
    Modify some API endpoints

    * `/api/telegram/otpVerification` ⇒ `/api/tg/otp`
    * `/api/email/otpVerification` ⇒ `/api/email/otp`
    * `/api/getData` ⇒ ∅[^4]

!!! warning "CHANGE"
    Modify request parameter components to API endpoints

    * `authkey` (Param) ⇒ `Authkey` (Header).
    * `chatid` (Param) ⇒ `ChatID` (Header).
    * `email` (Param) ⇒ `Email` (Header).

[^1]: We'll have separate documentation on the **`X.509`** certificate information used in the upcoming version of **/AuthKit API v2**.

[^2]: This is the public **`X.509`** certificate file format created for **/AuthKit API v2**. You can obtain it by exporting the `.avc-pubcert` file via **AVCManager**.

[^3]: This is the private **`X.509`** certificate file format created for **/AuthKit API v2**. You can obtain it by exporting the `.avc-privcert` file via **AVCManager**.

[^4]: This API will be migrated to **AVCManager**

