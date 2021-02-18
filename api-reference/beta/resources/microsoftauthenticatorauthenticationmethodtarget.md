---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8eb9959faaf5f4a6bcaecceb165384be737623d
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292275"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД объекта пользователя или группы Azure AD.|
|isNumberMatchingRequired (private Preview)|Логический|Требовать от пользователя совпадения номера, отображаемого на странице для регистрации, чтобы утвердить уведомление MFA.|
|isRegistrationRequired|Логический|Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности. *Не поддерживается.* |
|shownContext (Private Preview)|authenticatorAppContextType|Определяет, какие типы контекста о входе должны показываться пользователю в теле уведомления. Возможные значения: `location`, `app`.|
|targetType|authenticationMethodTargetType| Возможные значения: `null`, `user`, `group`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String",
  "isNumberMatchingRequired": "Boolean"
}
```

