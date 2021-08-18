---
title: тип ресурса deliveryOptimizationBandwidthBusinessHoursLimit
description: Тип бизнес-часов и процентов пропускной способности
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60e78ee837702a1a131ee0abba46029186f4dfcfe4eab777eca4e5377defdb60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122665"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>тип ресурса deliveryOptimizationBandwidthBusinessHoursLimit

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип бизнес-часов и процентов пропускной способности

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|Указывает начало часов работы с помощью 24-часовой стрелки (0-23). Допустимые значения от 0 до 23|
|bandwidthEndBusinessHours|Int32|Указывает конец часов работы с помощью 24-часовой стрелки (0-23). Допустимые значения от 0 до 23|
|bandwidthPercentageDuringBusinessHours|Int32|Указывает процент пропускной способности для ограничения в часы работы (0-100). Допустимые значения: от 0 до 100|
|bandwidthPercentageOutsideBusinessHours|Int32|Указывает процент пропускной способности, чтобы ограничить время работы outsidse (0-100). Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```




