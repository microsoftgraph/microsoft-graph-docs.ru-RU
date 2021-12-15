---
title: тип ресурса bookingStaffMemberBase
description: Абстрактный базовый тип для сотрудников Bookings.
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 17d13e80cf61e1cc885b07666708c9f8f479a385
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526755"
---
# <a name="bookingstaffmemberbase-resource-type"></a>тип ресурса bookingStaffMemberBase

Пространство имен: microsoft.graph

Абстрактный базовый тип для сотрудников Bookings.

Базовый тип [bookingStaffMember](bookingstaffmember.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID сотрудника. Наследуется от [сущности](../resources/entity.md).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingStaffMemberBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingStaffMemberBase",
  "id": "String (identifier)"
}
```

