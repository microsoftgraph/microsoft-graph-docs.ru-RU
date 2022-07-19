---
title: Тип ресурса staffAvailabilityItem
description: Представляет доступные и занятые интервалы времени сотрудника Bookings.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2737d50eb65d0cdf4d0e44f3df76038968399f93
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856452"
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
  "availabilityItems": [{"@odata.type": "microsoft.graph.availabilityItem"}],
  "staffId": "String"
}
```