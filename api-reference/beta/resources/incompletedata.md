---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549036"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса Инкомплетедата

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.
Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| Миссингдатабефоредатетиме | DateTimeOffset | В службе нет исходных данных до указанного времени.
| Вассроттлед              | Логический        | Некоторые данные не были записаны из-за чрезмерной активности.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
