---
title: Тип ресурса Букингкурренци
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f4b5cc6a8fdb36c2e4543302ac32846a1b3c4388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071796"
---
# <a name="bookingcurrency-resource-type"></a>Тип ресурса Букингкурренци

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет денежную валюту, поддерживаемую [букингбусинесс](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список БукингкурренЦиес](../api/bookingcurrency-list.md) | Коллекция [букингкурренци](bookingcurrency.md) |Получение списка объектов **букингкурренци** , доступных для корпоративных книг Майкрософт.|
|[Получение Букингкурренци](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Получение свойств объекта **букингкурренци** .|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| 3-значный код валюты, основанный на [стандарте ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Например, код валюты для доллара США равен USD, а Австралийский доллар — ауд. Только для чтения.|
|знаки|String| Символ валюты. Например, символ денежной единицы для доллара США и Австралийский доллар — $.  |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


