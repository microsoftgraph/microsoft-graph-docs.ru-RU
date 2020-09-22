---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ae3add0c3541e1617fec6bb71f0e05bb8fdc1b3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016683"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| description    | String | Описание организации.                                                         |
| displayName    | String | Отображаемое имя Организации.                                                        |
| externalSource | String | Источник для создания пользователя. Возможные значения: `sis` , `lms` , или `manual` . |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


