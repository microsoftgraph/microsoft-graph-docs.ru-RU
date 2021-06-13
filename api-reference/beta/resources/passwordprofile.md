---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: 47c55261316f2d85d27a4c993b358676578e74fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911335"
---
# <a name="passwordprofile-resource-type"></a>Тип ресурса passwordProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| Если при следующем входе пользователь `true` должен изменить пароль. После изменения пароля это свойство будет автоматически сброшено на * `false` . Если не установлено, по умолчанию `false` . |
|forceChangePasswordNextSignInWithMfa|Boolean| Если при следующем входе пользователь должен выполнить многофакторную проверку подлинности (MFA), прежде чем его принудить `true` изменить пароль. Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля. После изменения пароля это свойство будет автоматически сброшено на `false` . Если не установлено, по умолчанию `false` . |
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


