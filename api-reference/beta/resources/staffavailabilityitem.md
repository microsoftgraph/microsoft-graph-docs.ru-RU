---
title: Тип ресурса staffAvailabilityItem
description: Представляет доступные и занятые интервалы времени для Bookings сотрудника.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5c130388ce2b728c22c467689b998ffe8673c718
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755753"
---
# <a name="staffavailabilityitem-resource-type"></a>Тип ресурса staffAvailabilityItem

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет доступные и занятые интервалы времени для Bookings [сотрудника](bookingstaffmember.md).

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
