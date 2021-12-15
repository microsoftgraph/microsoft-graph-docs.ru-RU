---
title: тип ресурса bookingNamedEntity
description: Это базовый тип для субъектов Microsoft Bookings, которые предоставляют имя отображения, например bookingBusiness, bookingPerson, bookingService.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9d0700f6ac86d16ad00684d429a0f88fdb7a16a7
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525290"
---
# <a name="bookingnamedentity-resource-type"></a>тип ресурса bookingNamedEntity

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Это базовый тип для субъектов Microsoft Bookings, которые предоставляют имя отображения, например [bookingBusiness,](bookingbusiness.md) [bookingPerson,](bookingperson.md) [bookingService,](bookingservice.md) [bookingCustomQuestion.](bookingcustomquestion.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Имя полученной сущности, которая взаимодействует с клиентами.|
|id|Строка| ID для полученного объекта. Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


