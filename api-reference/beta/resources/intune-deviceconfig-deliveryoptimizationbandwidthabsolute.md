---
title: Тип ресурса Деливерйоптимизатионбандвидсабсолуте
description: Пределы проПускной способности в килобайтах в секунду.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178271"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсабсолуте

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пределы проПускной способности в килобайтах в секунду.


НаСледуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Максимумдовнлоадбандвидсинкилобитесперсеконд|Int64|Указывает максимальную пропускную способность скачивания в килобайтах/с, которую устройство может использовать для всех параллельных операций загрузки с помощью оптимизации доставки. Допустимые значения — от 0 до 4294967295
Значение 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загружаемых файлов. Допустимые значения — от 0 до 4294967295|
|Максимумуплоадбандвидсинкилобитесперсеконд|Int64|Указывает максимальную пропускную способность передачи в килобайтах/с, которая будет использоваться устройством для всех параллельных операций отправки с помощью оптимизации доставки (0-4000000). Допустимые значения — от 0 до 4000000
Значение по умолчанию — 0, что позволяет использовать неограниченную пропускную способность (оптимизирована для минимального использования полосы пропускания при загрузке). Допустимые значения — от 0 до 4000000|

## <a name="relationships"></a>Отношения
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




