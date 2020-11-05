---
title: Общие сведения об API политики проверки подлинности в Azure AD
description: Методы проверки подлинности политики определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 730368b4e47c34353882e5e601644133dbb38225
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921573"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Общие сведения о политиках методов проверки подлинности в Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Методы проверки подлинности политики определяют [методы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) и пользователей, которым разрешено использовать их для входа и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). Методы проверки подлинности, которые могут управляться в Microsoft Graph, включают ключи безопасности FIDO2 и мобильный вход с помощью приложения Microsoft Authenticator.

Для управления параметрами политики используются API политик метода проверки подлинности. Пример:

* Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
* Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без пароля, чтобы войти в Azure AD.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Какие политики способов проверки подлинности могут управляться в Microsoft Graph?

|Политика метода проверки подлинности       | Описание |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Определите ограничения ключа безопасности FIDO2 и пользователей, которые могут использовать их для входа в Azure AD.|
|[пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать вход без пароля, чтобы войти в Azure AD.|

## <a name="next-steps"></a>Дальнейшие действия

* опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
