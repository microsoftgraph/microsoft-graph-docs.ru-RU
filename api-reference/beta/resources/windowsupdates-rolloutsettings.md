---
title: тип ресурса rolloutSettings
description: Параметры, как служба развертывает обновление со временем.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 398bfdf0a33829f64a6b06de098cfc07a5df835e
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792003"
---
# <a name="rolloutsettings-resource-type"></a>тип ресурса rolloutSettings

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, как служба развертывает обновление со временем.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Дата, с которой устройства в развертывании начинают получать обновление. Если не установлено, развертывание начинается сразу после назначения устройств.|
|devicesPerOffer|Int32| Указывает количество устройств, предлагаемых одновременно. Не влияет при **наборе endDateTime.** Если **endDateTime и** **devicesPerOffer** не настроены, все устройства в развертывании одновременно предлагают контент.|
|durationBetweenOffers|String|Указывает продолжительность между каждым набором устройств, которые предлагают обновление. Оказывает влияние при определении **endDateTime** или **devicesPerOffer.** Значение по умолчанию `P1D` (1 день).|
|endDateTime|DateTimeOffset|Указывает дату, до которой всем устройствам в развертывании предлагается обновление. Устройства, добавленные после этой даты, предлагаются немедленно. Если **endDateTime и** **devicesPerOffer** не настроены, все устройства в развертывании одновременно предлагают контент.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```

