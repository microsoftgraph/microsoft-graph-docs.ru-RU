---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: a597b17d09414a839cb0c8d0ae3c944c255ae8ec
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208325"
---
# <a name="passwordprofile-resource-type"></a>Тип ресурса passwordProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**. См. пример [обновления passwordProfile пользователя.](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean|  Значение `true` указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение `false`. Если значение не задано, по умолчанию используется `false`. **ПРИМЕЧАНИЕ.** Для клиентов Azure B2C присвойте значение `false` и вместо этого используйте настраиваемые политики и пользовательские потоки для принудительного сброса пароля при первом входе. См. раздел [Принудительный сброс пароля при первом входе](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon). |
|forceChangePasswordNextSignInWithMfa|Boolean| Если присвоено значение `true`, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля. Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что перед изменением пароля пользователю нужно выполнить многофакторную проверку подлинности. После изменения пароля это свойство автоматически сбрасывается до значения `false`. Если значение не задано, по умолчанию используется `false`. |
|password|Строка|Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


