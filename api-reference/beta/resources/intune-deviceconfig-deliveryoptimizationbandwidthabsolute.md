---
title: deliveryOptimizationBandwidthAbsolute resource type
description: Ограничения пропускной способности в килобайтах в секунду.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8d625892c0d8651de284037d5a2ba4158a3b34a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147992"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute resource type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения пропускной способности в килобайтах в секунду.


Наследует от [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|Указывает максимальную пропускную способность загрузки в KiloBytes/second, которую устройство может использовать во всех одновременно загружаемых действиях с помощью оптимизации доставки. Допустимые значения от 0 до 4294967295
Значение 0 (ноль) означает, что оптимизация доставки динамически настраивается на использование доступной пропускной способности для скачивания. Допустимые значения от 0 до 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|Указывает максимальную пропускную способность загрузки в KiloBytes/second, которую устройство будет использовать во всех параллельной загрузке с помощью оптимизации доставки (0-4000000). Допустимые значения от 0 до 4000000
Значение по умолчанию — 0, что позволяет неограниченное количество пропускной способности (оптимизировано для минимального использования пропускной способности загрузки). Допустимые значения от 0 до 4000000|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```



