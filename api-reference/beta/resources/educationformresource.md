---
title: Тип ресурса Едукатионформресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является формой.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f2747d94c80732091db06294b26546afc567e03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334267"
---
# <a name="educationformresource-resource-type"></a>Тип ресурса Едукатионформресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Этот ресурс является формой.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Оригиналформид|String|Исходный идентификатор формы.|
|Формид|String|Идентификатор формы.|
|Исграупформ|Логический|Принадлежность формы группе классов.|
|Виевурл|String|URL-адрес студента для формы.|
|Виевурл|String|URL-адрес студента для формы.|
|Едитурл|String|URL-адрес преподавателя для формы.|

## <a name="json-representation"></a>Представление JSON

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
