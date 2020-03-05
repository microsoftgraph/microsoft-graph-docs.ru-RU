---
title: Тип ресурса Букингкустомер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: af64f8686b1779030c0ace93b4805845c6ed3c81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507998"
---
# <a name="bookingcustomer-resource-type"></a>Тип ресурса Букингкустомер

Пространство имен: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет клиента объекта [букингбусинесс](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление клиентов](../api/bookingbusiness-list-customers.md) | Коллекция [букингкустомер](bookingcustomer.md) | Получение списка объектов **букингкустомер** . |
|[Создание Букингкустомер](../api/bookingbusiness-post-customers.md) | [букингкустомер](bookingcustomer.md) | Создание нового объекта **букингкустомер** . |
|[Получение Букингкустомер](../api/bookingcustomer-get.md) | [букингкустомер](bookingcustomer.md) |Чтение свойств и связей объекта **букингкустомер** .|
|[обновление](../api/bookingcustomer-update.md). | [букингкустомер](bookingcustomer.md) |Обновление объекта **букингкустомер** . |
|[удаление](../api/bookingcustomer-delete.md); | Нет |Удаление объекта **букингкустомер** . |

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
