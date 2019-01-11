---
title: Тип ресурса bookingCurrency
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 96a5e04f705cca04e926ce25fd7e674528a60ccb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843675"
---
# <a name="bookingcurrency-resource-type"></a>Тип ресурса bookingCurrency

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет денежных валюты, поддерживаемый [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список bookingCurrencies](../api/bookingcurrency-list.md) | [bookingCurrency](bookingcurrency.md) коллекции |Получите список объектов **bookingCurrency** , доступные для резервирования Microsoft business.|
|[Получение bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Получение свойств объекта **bookingCurrency** .|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Код 3-символ валюты, на основании [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). К примеру код валюты доллара США — долларов США, а для Австралии доллар — AUD. Только для чтения.|
|символ|Строка| Символ валюты. Например символ валюты доллара США, а также для Австралии доллар — $.  |

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
