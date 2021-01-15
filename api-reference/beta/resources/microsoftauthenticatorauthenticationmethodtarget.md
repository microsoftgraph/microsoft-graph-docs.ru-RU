---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 395a1a10d9d99ce8ea5475e09a2e082b3bc5ddf3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874496"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД объекта пользователя или группы Azure AD.|
|isNumberMatchingRequired (Private Preview)|Boolean|Требовать от пользователя совпадения номера, отображаемого на странице для регистрации, чтобы утвердить уведомление MFA.|
|isRegistrationRequired|Boolean|Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности. *Не поддерживается.* |
|shownContext (Private Preview)|authenticatorAppContextType|Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления. Возможные значения: `location`, `app`.|
|targetType|authenticationMethodTargetType| Возможные значения: `user`, `group`.|

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

