---
title: Обзор API политики проверки подлинности Azure AD
description: 'Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.'
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
---

# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Обзор API политик проверки подлинности Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).[](/azure/active-directory/authentication/concept-authentication-methods) Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и Телефон вход с Microsoft Authenticator приложением.

API-политики методов проверки подлинности используются для управления настройками политики. Например:

* Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
* Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или Телефон для регистрации в Azure AD.
* Определите пользователей или группы пользователей, которым следует напомнить о Microsoft Authenticator для MFA с помощью push-уведомлений.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Какие политики методов проверки подлинности можно управлять в Microsoft Graph?

|Политика метода проверки подлинности       | Описание |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| Определите пользователей, которые могут использовать текстовое сообщение в клиенте Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Определите ограничения ключей безопасности FIDO2 и пользователей, которые могут использовать их для входов в Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Определите пользователей, которые могут Microsoft Authenticator в клиенте Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать OTP электронной почты в клиенте Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)|Определите пользователей, которые могут использовать Телефон для регистрации в Azure AD.|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать временный пропуск доступа для входов в Azure AD.|
|[x509CertificateAuthenticationMethodConfiguration](x509CertificateAuthenticationMethodConfiguration.md)|Определите пользователей, которые могут использовать сертификат X.509 для регистрации в Azure AD.|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a>Политики, доступные для того, чтобы подтолкнуть пользователей к настройкам методов проверки подлинности:
|Политика       | Описание |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| Определите пользователей, которым следует напомнить о том, как настроить метод проверки подлинности (поддерживается только для Microsoft Authenticator).|

## <a name="next-steps"></a>Дальнейшие действия

* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
