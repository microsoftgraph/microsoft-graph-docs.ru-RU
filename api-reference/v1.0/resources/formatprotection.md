---
title: Тип ресурса formatProtection
description: Представляет защиту формата объекта Range.
ms.localizationpriority: medium
author: ruoyingl
ms.prod: workbooks-and-charts
doc_type: resourcePageType
ms.openlocfilehash: 592699a23a7a418faa8e9679111b41c0eb964b2f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900459"
---
# <a name="formatprotection-resource-type"></a>Тип ресурса formatProtection

Пространство имен: microsoft.graph

Представляет защиту формата объекта Range.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта FormatProtection](../api/formatprotection-get.md) | [FormatProtection](formatprotection.md) |Чтение свойств и связей объекта formatProtection.|
|[Обновление](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |Обновление объекта FormatProtection. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|formulaHidden|boolean|Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.|
|locked|boolean|Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

