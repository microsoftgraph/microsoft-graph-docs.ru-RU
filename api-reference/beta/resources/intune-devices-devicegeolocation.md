---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acf2987e7c022754ff0659d82027b4d0d26901bd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772176"
---
# <a name="devicegeolocation-resource-type"></a>Тип ресурса deviceGeoLocation

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расположение устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Ластколлектеддатетимеутк|DateTimeOffset|Время записи расположения относительно времени UTC|
|lastCollectedDateTime|DateTimeOffset|Время записи расположения относительно времени UTC|
|longitude|Двойное с плавающей точкой|Долгота расположения устройства|
|latitude|Двойное с плавающей точкой|Широта расположения устройства|
|altitude|Двойное с плавающей точкой|Высота (метров над уровнем моря)|
|horizontalAccuracy|Двойное с плавающей точкой|Точность долготы и широты (м)|
|verticalAccuracy|Двойное с плавающей точкой|Точность высоты (м)|
|heading|Двойное с плавающей точкой|Направление от географического севера (градусов)|
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





