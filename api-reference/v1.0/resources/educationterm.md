---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947584"
---
# <a name="educationterm-resource-type"></a>Тип ресурса educationTerm

Срок. Представляет определенную часть учебного года. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName| String| Отображаемое имя срока.| 
|externalId|String| Идентификатор срока в системе синхронизации.|
|startDate|Date|Начало срока.|
|endDate|Date|Конец срока.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
