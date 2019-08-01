---
title: Тип ресурса educationOrganization
description: Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c62e65ffb6c6a0e3a8af92bda6a8b1e1c241ada7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032636"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String| Описание организации.|
|displayName|Строка| Отображаемое имя Организации.|
|externalSource|Едукатионекстерналсаурце| Источник, из которого была создана данная организация. Допустимые значения: `sis`, `manual`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
