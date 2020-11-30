---
title: Тип ресурса Клаудпконпремисесконнектионстатусдетаилс
description: Сведения о состоянии локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 19dedd3344d5ed049a5b6ff5361ed7a8e4937146
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378461"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a>Тип ресурса Клаудпконпремисесконнектионстатусдетаилс

Пространство имен: microsoft.graph

Сведения о состоянии [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Время начала проверки работоспособности подключения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|endDateTime|DateTimeOffset|Время окончания проверки работоспособности подключения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|хеалсчеккс|Коллекция [клаудпконпремисесконнектионхеалсчекк](../resources/cloudpconpremisesconnectionhealthcheck.md)|Все проверки, выполняемые для подключения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```
