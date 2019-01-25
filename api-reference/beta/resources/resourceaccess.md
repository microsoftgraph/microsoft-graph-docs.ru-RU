---
title: Тип ресурса resourceAccess
description: Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа requiredResourceAccess — это коллекция **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519026"
---
# <a name="resourceaccess-resource-type"></a>Тип ресурса resourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Guid|Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md) , которые предоставляет доступ к приложению ресурсов.|
|type|String|Указывает, будет ли свойство **id** ссылается на [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md). Возможные значения: «область» или «роли».|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
