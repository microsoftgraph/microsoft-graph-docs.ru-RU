---
title: Обзор API политики методов проверки подлинности Azure AD
description: Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использовать пользователи в Azure AD.
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 593cbea196edcbe1c868a337b1dcfa8a1de2afc9
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271829"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Обзор API политик методов проверки подлинности Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которые могут использовать их для выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). [](/azure/active-directory/authentication/concept-authentication-methods) Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и вход без пароля с помощью приложения Microsoft Authenticator.

API политик методов проверки подлинности используются для управления настройками политики. Например:

* Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
* Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход в Azure AD без пароля.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Какими политиками методов проверки подлинности можно управлять в Microsoft Graph?

|Политика методов проверки подлинности       | Описание |
|:---------------------------|:------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| Определите пользователей, которые могут использовать sms-сообщения в клиенте Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Определите ограничения клавиш безопасности FIDO2 и пользователей, которые могут использовать их для входов в Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать Microsoft Authenticator в клиенте Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать OTP электронной почты в клиенте Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (неподдерживаемая)|Определите пользователей, которые могут использовать для входов в Azure AD телефонный вход без пароля.|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать временный доступ для входов в Azure AD.|

## <a name="next-steps"></a>Дальнейшие действия

* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
