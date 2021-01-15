---
title: Обзор API методов проверки подлинности Azure AD
description: Методы проверки подлинности — это способ проверки подлинности пользователей в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 98de9847ec0e50cb17c6ab64423d891bd3c5e8a3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874307"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Обзор API методов проверки подлинности Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Методы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (AD). Способы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которыми можно управлять в Microsoft Graph уже сегодня, и множество других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).

API метода проверки подлинности используются для управления методами проверки подлинности пользователя. Пример:

* Вы можете добавить номер телефона для пользователя. Затем пользователь может использовать этот номер телефона для проверки подлинности sms и голосовых вызовов, если он включен для использования политикой.
* Вы можете обновить этот номер или удалить его у пользователя.
* Вы можете включить или отключить номер для sms-входов.
* Вы можете сбросить пароль пользователя.
* Вы можете получить сведения о ключе безопасности FIDO2 пользователя и удалить его, если пользователь потеряет ключ.
* Вы можете получить сведения о регистрации пользователя Microsoft Authenticator и удалить его, если пользователь потеряет телефон.
* Вы можете добавить адрес электронной почты для пользователя. Затем пользователь может использовать это сообщение электронной почты в процессе Self-Service сброса пароля (SSPR).
* Вы можете обновить это сообщение электронной почты или удалить его у пользователя.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Какими методами проверки подлинности можно управлять в Microsoft Graph?

|Способ проверки подлинности        | Описание |Примеры     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| Пароль в настоящее время является основным методом проверки подлинности по умолчанию в Azure AD.|сбросить пароль пользователя.|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|Пользователь может использовать телефон для проверки подлинности с помощью [SMS](/azure/active-directory/authentication/concept-authentication-methods#phone-options) или голосовых вызовов (разрешено политикой).|См. телефонные номера для проверки подлинности пользователя. Добавление, обновление или удаление номера телефона для пользователя. Включить или отключить основной мобильный телефон для sms-входов.|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Пользователь может использовать ключ безопасности FIDO2 для входов в Azure AD.|Удаление утерянного ключа безопасности FIDO2.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Пользователь может использовать Microsoft Authenticator для выполнения многофакторной проверки подлинности в Azure AD|Удаление метода проверки подлинности Microsoft Authenticator.|
|[passwordlessmicrosoftauthenticatorauthenticationmethod](passwordlessmicrosoftauthenticatorauthenticationmethod.md) (неподготовлен)|Пользователь может войти в Azure AD с помощью microsoft Authenticator Phone Sign-in|Удаление метода проверки подлинности для телефона без пароля.|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|Адрес электронной почты может быть пользователем в рамках процесса Self-Service сброса пароля (SSPR).|См. адрес электронной почты для проверки подлинности пользователя. Добавление, обновление или удаление адреса электронной почты для пользователя.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello для бизнеса — это метод входов без пароля на устройствах с Windows.|См. устройства, на которых пользователь включил вход в Windows Hello для бизнеса. Удаление учетных данных Windows Hello для бизнеса.|

## <a name="next-steps"></a>Дальнейшие действия

* Просмотрите типы методов проверки подлинности и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).