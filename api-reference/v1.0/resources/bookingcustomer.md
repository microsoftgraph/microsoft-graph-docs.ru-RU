---
title: тип ресурса bookingCustomer
description: Представляет клиента bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fa9bf3e9ebe49857972635dc87c604d066b6da12
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526892"
---
# <a name="bookingcustomer-resource-type"></a>тип ресурса bookingCustomer

Пространство имен: microsoft.graph

Представляет клиента [bookingBusiness](bookingbusiness.md).

Наследует от [bookingCustomerBase](bookingcustomerbase.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список клиентов](../api/bookingbusiness-list-customers.md) | [коллекция bookingCustomer](bookingcustomer.md) | Получите список объектов **bookingCustomer.** |
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Создайте новый **объект bookingCustomer.** |
|[Get bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Ознакомьтесь с свойствами и отношениями объекта **bookingCustomer.**|
|[Обновление](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Обновление **объекта bookingCustomer.** |
|[удаление](../api/bookingcustomer-delete.md); | Нет |Удаление **объекта bookingCustomer.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Имя клиента.|
|emailAddress|String|SMTP-адрес клиента.|
|id|Строка| ID клиента. Только для чтения.|
|addresses|[коллекция physicalAddress](../resources/physicaladdress.md)|Адреса, связанные с клиентом. Тип **атрибута** physicalAddress не поддерживается в v1.0. Внутренне мы относям адреса к типу `others` .|
|phones|Коллекция [phone](../resources/phone.md)|Телефон номеров, связанных с клиентом, включая домашние, деловые и мобильные номера.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer",
  "baseType": "microsoft.graph.bookingCustomerBase"
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


