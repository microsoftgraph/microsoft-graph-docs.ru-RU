---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd7035bbd57e8deb5e80fdc4cfa770c559e30ef0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526806"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже

Пространство имен: Microsoft. Graph

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



