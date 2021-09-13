---
title: deliveryOptimizationBandwidthHoursWithPercentage type
description: Ограничение пропускной способности в процентах с бизнес-часами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88d21f6c2d73aa0fc4ad362f276994d1e5d3d4a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147978"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a>deliveryOptimizationBandwidthHoursWithPercentage type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение пропускной способности в процентах с бизнес-часами.


Наследует от [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bandwidthBackgroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Процентные часы загрузки фона.|
|bandwidthForegroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Процентные часы загрузки переднего плана.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```



