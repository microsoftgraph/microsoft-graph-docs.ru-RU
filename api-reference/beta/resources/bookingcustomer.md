---
title: Тип ресурса Букингкустомер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f97f3d36599fe088f28176d001fecc701bb5e3ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339085"
---
# <a name="bookingcustomer-resource-type"></a>Тип ресурса Букингкустомер

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет клиента объекта [букингбсинесс](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[ПереЧисление клиентов](../api/bookingbusiness-list-customers.md) | Коллекция [букингкустомер](bookingcustomer.md) | Получение списка объектов **букингкустомер** . |
|[Создание Букингкустомер](../api/bookingbusiness-post-customers.md) | [Букингкустомер](bookingcustomer.md) | Создание нового объекта **букингкустомер** . |
|[Получение Букингкустомер](../api/bookingcustomer-get.md) | [Букингкустомер](bookingcustomer.md) |Чтение свойств и связей объекта **букингкустомер** .|
|[Update](../api/bookingcustomer-update.md) | [Букингкустомер](bookingcustomer.md) |Обновление объекта **букингкустомер** . |
|[Delete](../api/bookingcustomer-delete.md) | Нет |Удаление объекта **букингкустомер** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Имя клиента.|
|emailAddress|String|SMTP-адрес клиента.|
|id|String| Идентификатор клиента. Только для чтения.|

## <a name="relationships"></a>Отношения
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
