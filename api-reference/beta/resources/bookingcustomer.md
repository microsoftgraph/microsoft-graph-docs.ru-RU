---
title: Тип ресурса Букингкустомер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 864635014b3e215dabd11896922ca9e73a5e8cb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974173"
---
# <a name="bookingcustomer-resource-type"></a>Тип ресурса Букингкустомер

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет клиента объекта [букингбусинесс](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление клиентов](../api/bookingbusiness-list-customers.md) | Коллекция [букингкустомер](bookingcustomer.md) | Получение списка объектов **букингкустомер** . |
|[Создание Букингкустомер](../api/bookingbusiness-post-customers.md) | [Букингкустомер](bookingcustomer.md) | Создание нового объекта **букингкустомер** . |
|[Получение Букингкустомер](../api/bookingcustomer-get.md) | [Букингкустомер](bookingcustomer.md) |Чтение свойств и связей объекта **букингкустомер** .|
|[обновление](../api/bookingcustomer-update.md); | [Букингкустомер](bookingcustomer.md) |Обновление объекта **букингкустомер** . |
|[Удаление](../api/bookingcustomer-delete.md) | Нет |Удаление объекта **букингкустомер** . |

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
