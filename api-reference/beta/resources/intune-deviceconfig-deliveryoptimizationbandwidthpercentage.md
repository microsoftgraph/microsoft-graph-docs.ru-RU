---
title: тип ресурса deliveryOptimizationBandwidthPercentage
description: Ограничения пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f1aab20ff6bbb7ab4e353e6d82fd2b19dd62281
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820459"
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



