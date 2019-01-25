---
title: Тип ресурса educationIdentityCreationConfiguration
description: Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511403"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Тип ресурса educationIdentityCreationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.

> **Примечание:** Если у вас есть синхронизации каталогов, включенным для синхронизации между локальной службы каталогов Active Directory и Azure Active Directory (Azure AD), используйте [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) ресурсов.

На основе [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md) коллекции |  Задает список доменов для использования каждого типа пользователя.  |


## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
