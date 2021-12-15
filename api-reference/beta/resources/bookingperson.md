---
title: Тип ресурса bookingPerson
description: Это базовый тип для человека в бизнесе Microsoft Bookings, который может быть bookingCustomer или bookingStaffMember.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 0ad4cd1d587fb2ccd88727f24944bc4226e43b7f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526186"
---
# <a name="bookingperson-resource-type"></a>Тип ресурса bookingPerson

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Это базовый тип для человека в бизнесе Microsoft Bookings, который может быть [bookingCustomer](bookingcustomer.md) или [bookingStaffMember](bookingstaffmember.md).

Наследует [от bookingNamedEntity](bookingnamedentity.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Имя полученной сущности, которая взаимодействует с клиентами. Наследуется **от bookingNamedEntity**.|
|emailAddress|String|Адрес электронной почты человека.|
|id|Строка| ID для полученного объекта. Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
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
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


