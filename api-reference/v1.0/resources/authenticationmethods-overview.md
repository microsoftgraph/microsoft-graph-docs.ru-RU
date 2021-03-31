---
title: Обзор API методов проверки подлинности Azure AD
description: Методы проверки подлинности — это проверка подлинности пользователями в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 6027e03a4c78c5359db77ee9c263c9e98f412a9f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469124"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Обзор API методов проверки подлинности Azure AD

Пространство имен: microsoft.graph

[Методы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователями в Azure Active Directory (AD). Методы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которые сегодня можно использовать в конечной точке бета-версии Microsoft Graph, среди многих других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).

API метода проверки подлинности используются для управления методами проверки подлинности пользователя. Например:

* Вы можете получить сведения о ключе безопасности FIDO2 пользователя и удалить его, если пользователь потерял ключ.
* Вы можете получить сведения о регистрации Microsoft Authenticator пользователя и удалить его, если пользователь потерял телефон.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Какие методы проверки подлинности можно управлять в Microsoft Graph?

|Способ проверки подлинности        | Описание |Примеры     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Ключ безопасности FIDO2 может быть использован пользователем для регистрации в Azure AD.|Удаление потерянного ключа безопасности FIDO2.|
|[MicrosoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator может использоваться пользователем для регистрации или выполнения многофакторной проверки подлинности в Azure AD|Удаление метода проверки подлинности Microsoft Authenticator.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello для бизнеса — это метод без паролей для регистрации на устройствах Windows.|См. устройства, на которых пользователь включил вход в Windows Hello для бизнеса. Удаление учетных данных Windows Hello для бизнеса.|

## <a name="next-steps"></a>Дальнейшие действия

* Просмотрите типы методов проверки подлинности и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).