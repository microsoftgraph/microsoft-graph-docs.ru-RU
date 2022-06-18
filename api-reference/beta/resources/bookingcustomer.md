---
title: Тип ресурса bookingCustomer
description: Представляет клиента bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7e4c31ec68cdda121dcb1f7954faa742746271fc
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160652"
---
# <a name="bookingcustomer-resource-type"></a>Тип ресурса bookingCustomer

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет клиента [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление клиентов](../api/bookingbusiness-list-customers.md) | [Коллекция bookingCustomer](bookingcustomer.md) | Получение списка объектов **bookingCustomer** . |
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Создайте объект **bookingCustomer** . |
|[Получение bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Чтение свойств и связей объекта **bookingCustomer** .|
|[Обновление](../api/bookingcustomer-update.md) | Нет  |Обновление объекта **bookingCustomer** . |
|[Удаление](../api/bookingcustomer-delete.md) | Нет |Удаление объекта **bookingCustomer** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|addresses|[Коллекция physicalAddress](../resources/physicaladdress.md)|Адреса, связанные с клиентом, включая домашние, бизнес-адреса и другие адреса.|
|displayName|Строка|Имя клиента.|
|emailAddress|String|SMTP-адрес клиента.|
|id|Строка| Идентификатор клиента. Только для чтения.|
|phones|Коллекция [phone](../resources/phone.md)|Телефон номера, связанные с клиентом, включая домашние, бизнес-номера и мобильные номера.|

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
  "id": "String (identifier)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ]
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


