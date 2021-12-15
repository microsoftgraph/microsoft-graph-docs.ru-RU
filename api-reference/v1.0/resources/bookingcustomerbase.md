---
title: тип ресурса bookingCustomerBase
description: Абстрактный базовый тип для клиентов Bookings.
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3eca954718608223977018b82f005001be269ba9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525133"
---
# <a name="bookingcustomerbase-resource-type"></a>тип ресурса bookingCustomerBase

Пространство имен: microsoft.graph

Абстрактный базовый тип для клиентов Bookings.

Базовый тип [bookingCustomer](bookingcustomer.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID клиента. Наследуется от [сущности](../resources/entity.md).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomerBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerBase",
  "id": "String (identifier)"
}
```

