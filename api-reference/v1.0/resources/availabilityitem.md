---
title: Тип ресурса availabilityItem
description: Указывает состояние сотрудника для заданного интервала времени.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a4a95c8954ce2541a6096f8fd31fd87517143060
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856448"
---
# <a name="availabilityitem-resource-type"></a>Тип ресурса availabilityItem

Пространство имен: microsoft.graph

Указывает состояние [сотрудника для](bookingstaffmember.md) заданного интервала времени.

## <a name="properties"></a>Свойства

| Свойство  | Тип |Описание|
|:---------------|:--------|:----------|
|endDateTime |dateTimeTimeZone |Время окончания интервала времени.|
|serviceId |Строка |Указывает идентификатор службы в случае 1:n встреч. Если встреча имеет тип 1:n, это поле будет присутствовать, в противном случае . `null`|
|status |bookingsAvailabilityStatus |Состояние сотрудника. Возможные значения: `available`, `busy`, `slotsAvailable`, `outOfOffice`, `unknownFutureValue`.|
|startDateTime |dateTimeTimeZone |Время начала интервала времени.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.availabilityItem"
}-->

``` json
{
  "endDateTime": "DateTimeInfo",
  "serviceId": "String",
  "status": "String",
  "startDateTime": "DateTimeInfo"
}
```