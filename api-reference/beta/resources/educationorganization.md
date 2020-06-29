---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 015b1c886f439e3c5952d1c1a5fcce02fb21773b
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909655"
---
# <a name="educationorganization-resource-type"></a>Тип ресурса educationOrganization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| description    | String | Описание организации.                                                         |
| displayName    | Строка | Отображаемое имя Организации.                                                        |
| externalSource | String | Источник для создания пользователя. Возможные значения: `sis` , `lms` , или `manual` . |

## <a name="relationships"></a>Связи

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
