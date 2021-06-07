---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a406ede926ad637a338437559840cdefdadc64ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754583"
---
# <a name="devicegeolocation-resource-type"></a>Тип ресурса deviceGeoLocation

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расположение устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|Время записи расположения относительно времени UTC|
|longitude|Double|Долгота расположения устройства|
|latitude|Double|Широта расположения устройства|
|altitude|Double|Высота (метров над уровнем моря)|
|horizontalAccuracy|Double|Точность долготы и широты (м)|
|verticalAccuracy|Double|Точность высоты (м)|
|heading|Double|Направление от географического севера (градусов)|
|speed|Double|Скорость передвижения устройства (м/с)|

## <a name="relationships"></a>Отношения
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
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "4.2",
  "latitude": "4.2",
  "altitude": "4.2",
  "horizontalAccuracy": "4.2",
  "verticalAccuracy": "4.2",
  "heading": "4.2",
  "speed": "4.2"
}
```




