---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: eketo-msft
ms.openlocfilehash: 4fdc58e79487b9577685929bb06865e3aca6906f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812487"
---
# <a name="passwordprofile-resource-type"></a>Тип ресурса passwordProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| Если задано **значение true**, при следующем входе пользователь должен изменить пароль. После смены пароля этому свойству будет автоматически присвоено значение ***false**. Если не установлено, по умолчанию используется значение **false**. |
|forceChangePasswordNextSignInWithMfa|Boolean| Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля. Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля. После изменения пароля это свойство автоматически сбрасывается до значения **false**. Если не установлено, по умолчанию используется значение **false**. |
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
