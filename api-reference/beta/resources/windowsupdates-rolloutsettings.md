---
title: тип ресурса rolloutSettings
description: Параметры, как служба развертывает обновление со временем.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 705eeae189d9159c07d3c115c77383a207eae6db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068076"
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

