---
title: Тип ресурса availabilityItem
description: Указывает состояние сотрудника для заданного интервала времени.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2b51fe3644fc6ca884d1eb4435a6b874f2293fa2
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755761"
---
# <a name="availabilityitem-resource-type"></a>Тип ресурса availabilityItem

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
