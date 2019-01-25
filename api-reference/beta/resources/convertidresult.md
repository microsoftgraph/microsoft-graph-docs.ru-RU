---
title: Тип ресурса convertIdResult
description: Результат преобразования формата код выполняется с помощью функции translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516527"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса convertIdResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат преобразования формата код выполняется с помощью функции [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| SourceId | String | Идентификатор, который был преобразован. Это значение является идентификатором исходного, без преобразованные. |
| targetId | String | Преобразованные идентификатор. Это значение не задано, если не удалось выполнить преобразование. |
| errorDetails | [Общая ошибка](genericerror.md) | Объект error, которое указывает причину сбоя преобразования. Это значение не задано, если преобразование выполнено успешно. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
