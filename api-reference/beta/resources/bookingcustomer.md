---
title: тип ресурса bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3d5eff9d0add4a0840e864b9f4caf1730be98e5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696233"
---
# <a name="bookingcustomer-resource-type"></a>тип ресурса bookingCustomer

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет клиента [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список клиентов](../api/bookingbusiness-list-customers.md) | [коллекция bookingCustomer](bookingcustomer.md) | Получите список объектов **bookingCustomer.** |
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Создайте новый **объект bookingCustomer.** |
|[Get bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Ознакомьтесь с свойствами и отношениями объекта **bookingCustomer.**|
|[Обновление](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Обновление **объекта bookingCustomer.** |
|[Удаление](../api/bookingcustomer-delete.md) | Нет |Удаление **объекта bookingCustomer.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Имя клиента.|
|emailAddress|String|SMTP-адрес клиента.|
|id|String| ID клиента. Только для чтения.|
|addresses|[коллекция physicalAddress](../resources/physicaladdress.md)|Адреса, связанные с клиентом, включая домашние, бизнес и другие адреса.|
|phones|Коллекция [phone](../resources/phone.md)|Телефон номеров, связанных с клиентом, включая домашние, деловые и мобильные номера.|

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


