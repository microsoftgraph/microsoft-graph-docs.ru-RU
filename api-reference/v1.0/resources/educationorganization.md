---
title: Тип ресурса educationOrganization
description: Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4f00fc4c44b3019dccbded1fd222aa211d78c7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032679"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

Пространство имен: microsoft.graph

Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String| Описание организации.|
|displayName|String| Отображаемое имя Организации.|
|externalSource|едукатионекстерналсаурце| Источник, из которого была создана данная организация. Допустимые значения: `sis`, `manual`, `unknownFutureValue`.|

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

