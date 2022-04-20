---
title: Тип ресурса staffAvailabilityItem
description: Представляет доступные и занятые интервалы времени для Microsoft Bookings сотрудника.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fa6a7e856060209f274c0503d3c0c27f567ae910
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917768"
---
# <a name="staffavailabilityitem-resource-type"></a>Тип ресурса staffAvailabilityItem

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет доступные и занятые интервалы времени для Microsoft Bookings [сотрудника](bookingstaffmember.md).

## <a name="properties"></a>Свойства

| Свойство  | Тип |Описание|
|:---------------|:--------|:----------|
|availabilityItems |[Коллекция availabilityItem](availabilityitem.md) |Каждый элемент в этой коллекции указывает слот и состояние сотрудника.|
|staffId |String |Идентификатор сотрудника.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.staffAvailabilityItem"
}-->

``` json
{
  "availabilityItems": "availabilityItem",
  "staffId": "String"
}
```
