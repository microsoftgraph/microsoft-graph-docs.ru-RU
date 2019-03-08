---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Корневой
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482373"
---
# <a name="root-resource-type"></a>Тип ресурса Root

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аспект **Root** указывает, что объект находится на верхнем уровне в иерархии.
Наличие ненулевого значения этого аспекта указывает, что объект является корневым элементом.
Значение null (или отсутствующее значение) указывает, что объект не является корневым.

**Примечание.** В настоящее время этот аспект пуст, но в будущих редакциях API он может быть дополнен другими свойствами.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>Свойства

У ресурса **Root** отсутствуют свойства.


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
