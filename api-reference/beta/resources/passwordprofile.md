---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
ms.openlocfilehash: a68cd61c7ab3fd1e62ca9bc889a6691068174dc6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574574"
---
# <a name="passwordprofile-resource-type"></a>Тип ресурса passwordProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| Если **значение true**, при следующем входе на, пользователь должен изменить пароль. После изменения пароля, это свойство будет автоматически изменено на ***значение false**. Если не задан, по умолчанию — **false**. |
|forceChangePasswordNextSignInWithMfa|Boolean| Если **значение true**, при следующем входе на, пользователь должен выполнить многофакторная проверка подлинности (многофакторной проверкой Подлинности) перед принудительно изменять свои пароли. Поведение идентично **forceChangePasswordNextSignIn** , за исключением того, что пользователь необходимо сначала выполнить многофакторной проверки подлинности до изменения пароля. После изменения пароля это свойство будет автоматически задано **значение false**. Если не задан, по умолчанию — **false**. |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
