---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395057"
---
# <a name="devicegeolocation-resource-type"></a>Тип ресурса deviceGeoLocation

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расположение устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|Время записи расположения относительно времени UTC|
|lastCollectedDateTime|DateTimeOffset|Время записи расположения относительно времени UTC|
|longitude|Double|Долгота расположения устройства|
|latitude|Double|Широта расположения устройства|
|altitude|Double|Высота (метров над уровнем моря)|
|horizontalAccuracy|Double|Точность долготы и широты (м)|
|verticalAccuracy|Double|Точность высоты (м)|
|heading|Double|Направление от географического севера (градусов)|
|speed|Double|Скорость передвижения устройства (м/с)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```




