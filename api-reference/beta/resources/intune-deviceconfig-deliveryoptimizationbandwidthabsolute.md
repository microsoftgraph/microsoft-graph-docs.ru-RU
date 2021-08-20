---
title: deliveryOptimizationBandwidthAbsolute resource type
description: Ограничения пропускной способности в килобайтах в секунду.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28aa1fa0ff3d305392842a4aae1ada0c2c3ad6954502430e94a7db9c8e7cf304
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241935"
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




