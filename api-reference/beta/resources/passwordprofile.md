---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
ms.openlocfilehash: 11930b046fafaf89f8db751891b9b7f2f72fd99d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839006"
---
# <a name="passwordprofile-resource-type"></a>Тип ресурса passwordProfile

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| Если **значение true**, при следующем входе на, пользователь должен изменить пароль. После изменения пароля, это свойство будет автоматически изменено на ***значение false**. Если не задан, по умолчанию — **false**. |
|forceChangePasswordNextSignInWithMfa|Логический| Если **значение true**, при следующем входе на, пользователь должен выполнить многофакторная проверка подлинности (многофакторной проверкой Подлинности) перед принудительно изменять свои пароли. Поведение идентично **forceChangePasswordNextSignIn** , за исключением того, что пользователь необходимо сначала выполнить многофакторной проверки подлинности до изменения пароля. После изменения пароля это свойство будет автоматически задано **значение false**. Если не задан, по умолчанию — **false**. |
|password|Строка|Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
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
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
