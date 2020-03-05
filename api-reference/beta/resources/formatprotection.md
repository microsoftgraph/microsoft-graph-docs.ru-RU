---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c574ceefd33131562a0df504fad26bb225056ce7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497820"
---
# <a name="formatprotection-resource-type"></a>Тип ресурса FormatProtection

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
