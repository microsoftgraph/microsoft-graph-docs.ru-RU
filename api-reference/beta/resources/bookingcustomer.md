---
title: Тип ресурса bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 1eef44dfe994238d654a21c5f26ec102dcf1881d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075864"
---
# <a name="bookingcustomer-resource-type"></a>Тип ресурса bookingCustomer

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет клиента [bookingBsiness](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список клиентов](../api/bookingbusiness-list-customers.md) | [bookingCustomer](bookingcustomer.md) коллекции | Получите список объектов **bookingCustomer** . |
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Создание нового объекта **bookingCustomer** . |
|[Получение bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Чтение свойства и связи объекта **bookingCustomer** .|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Обновление объекта **bookingCustomer** . |
|[Delete](../api/bookingcustomer-delete.md) | Нет |Удалите объект **bookingCustomer** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Имя клиента.|
|emailAddress|String|SMTP-адрес клиента.|
|id|String| Идентификатор клиента. Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->