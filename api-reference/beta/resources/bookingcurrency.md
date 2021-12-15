---
title: тип ресурса bookingCurrency
description: Представляет денежную валюту, поддерживаемую bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 80da1bddcc58965fc403f24b3242b34ca5c28f98
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525969"
---
# <a name="bookingcurrency-resource-type"></a>тип ресурса bookingCurrency

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет денежную валюту, поддерживаемую [bookingBusiness.](bookingbusiness.md)


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список bookingCurrencies](../api/bookingcurrency-list.md) | [коллекция bookingCurrency](bookingcurrency.md) |Получите список объектов **bookingCurrency,** доступных для бизнеса Microsoft Bookings.|
|[Получить bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Получите свойства объекта **bookingCurrency.**|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Код 3-символов валюты, основанный на [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Например, код валюты для доллара США — USD, а для австралийского доллара — AUD. Только для чтения.|
|символ|Строка| Символ валюты. Например, символ валюты для доллара США и австралийского доллара — $.  |

## <a name="relationships"></a>Связи
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


