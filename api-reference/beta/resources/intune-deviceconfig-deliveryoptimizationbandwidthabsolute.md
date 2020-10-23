---
title: Тип ресурса Деливерйоптимизатионбандвидсабсолуте
description: Пределы пропускной способности в килобайтах в секунду.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 710553bb01eb335eed9cf4075af3d87985239f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696253"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсабсолуте

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пределы пропускной способности в килобайтах в секунду.


Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|максимумдовнлоадбандвидсинкилобитесперсеконд|Int64|Указывает максимальную пропускную способность скачивания в килобайтах/с, которую устройство может использовать для всех параллельных операций загрузки с помощью оптимизации доставки. Допустимые значения — от 0 до 4294967295
Значение 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загружаемых файлов. Допустимые значения — от 0 до 4294967295|
|максимумуплоадбандвидсинкилобитесперсеконд|Int64|Указывает максимальную пропускную способность передачи в килобайтах/с, которая будет использоваться устройством для всех параллельных операций отправки с помощью оптимизации доставки (0-4000000). Допустимые значения — от 0 до 4000000
Значение по умолчанию — 0, что позволяет использовать неограниченную пропускную способность (оптимизирована для минимального использования полосы пропускания при загрузке). Допустимые значения — от 0 до 4000000|

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





