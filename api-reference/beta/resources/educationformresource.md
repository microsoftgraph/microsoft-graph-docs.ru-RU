---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0c8748c725f7289eadbca8119b47bf8a81b28c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095448"
---
# <a name="educationformresource-resource-type"></a>Тип ресурса Едукатионформресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Этот ресурс является формой.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|оригиналформид|Строка|Исходный идентификатор формы.|
|формид|Строка|Идентификатор формы.|
|исграупформ|Boolean|Принадлежность формы группе классов.|
|виевурл|Строка|URL-адрес студента для формы.|
|виевурл|Строка|URL-адрес студента для формы.|
|едитурл|Строка|URL-адрес преподавателя для формы.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


