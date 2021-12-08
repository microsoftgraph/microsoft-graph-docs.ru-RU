---
title: тип ресурса metricTimeSeriesDataPoint
description: Точка данных серии "Метрики"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e67e5bb60fc3b4c365ca7671cb57037687eb141
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347328"
---
# <a name="metrictimeseriesdatapoint-resource-type"></a>тип ресурса metricTimeSeriesDataPoint

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Точка данных серии "Метрики"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dateTime|DateTimeOffset|Время точки данных метрических рядов времени|
|значение|Int64|Значение точки данных метрических рядов времени|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.metricTimeSeriesDataPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.metricTimeSeriesDataPoint",
  "dateTime": "String (timestamp)",
  "value": 1024
}
```




