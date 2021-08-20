---
title: тип ресурса deliveryOptimizationBandwidthPercentage
description: Ограничения пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa03a71cbad86b181d3643c3bef9874159d47a299a8c51973a3238fecceeb5a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145462"
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




