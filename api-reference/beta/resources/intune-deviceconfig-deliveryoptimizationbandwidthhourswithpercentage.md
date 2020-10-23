---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fb685f87e602eb6312d3e80e441b2c064ec327b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696232"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предельная пропускная способность в процентах с рабочими часами.


Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|бандвидсбаккграундперцентажехаурс|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Процент загрузки в фоновом режиме.|
|бандвидсфореграундперцентажехаурс|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Процентное соотношение загрузки в процентах.|

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





