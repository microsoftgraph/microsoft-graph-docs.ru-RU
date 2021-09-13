---
title: тип ресурса deliveryOptimizationBandwidthPercentage
description: Ограничения пропускной способности, указанные в процентах.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd7efc4fdcee3a827239f368a5854ee7965a4e2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147964"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a>тип ресурса deliveryOptimizationBandwidthPercentage

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения пропускной способности, указанные в процентах.


Наследует от [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|maximumBackgroundBandwidthPercentage|Int32|Указывает максимальную пропускную способность загрузки фона, которую оптимизация доставки использует во всех одновременно загружаемых действиях в процентах от доступной пропускной способности загрузки (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически настраивает использование доступной пропускной способности для фоновых загрузок. Допустимые значения: от 0 до 100|
|maximumForegroundBandwidthPercentage|Int32|Указывает максимальную пропускную способность загрузки на переднем плане, которую оптимизация доставки использует во всех одновременно загружаемых действиях в процентах от доступной пропускной способности загрузки (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически настраивает использование доступной пропускной способности для загрузки переднего плана. Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



