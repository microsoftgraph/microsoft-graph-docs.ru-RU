---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513706"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Тип ресурса educationIdentityMatchingOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| appliesTo | string |  Тип роли пользователя для назначения лицензий. Возможные значения: `student`, `teacher`.      |
| **sourcePropertyName** | string |  Имя свойства источника, которое должно быть имя поля в источнике данных. Это свойство соответствует с учетом регистра.        |
| **targetPropertyName** | string |  Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD. Это свойство соответствует с учетом регистра.     |
| **targetDomain** | string |  Домен суффикс со свойством источника для сопоставления в целевой системе. Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.        |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
