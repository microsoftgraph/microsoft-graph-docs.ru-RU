---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507100"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>Тип ресурса Едукатионсинчронизатионлиценсеассигнмент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Тег** | строка | Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`.         |
| **Скуидс** | Коллекция строк |  Представляет идентификаторы SKU назначаемых лицензий.        |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
