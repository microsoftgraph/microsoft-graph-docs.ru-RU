---
title: тип ресурса timeSeriesParameter
description: Параметр передается в GetHealthMetricTimeSeries при запросе серии моментального снимка.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da593d882a0ab4fb4681c06bbb1c40cbb03a86ba
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58762996"
---
# <a name="timeseriesparameter-resource-type"></a>тип ресурса timeSeriesParameter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр передается в GetHealthMetricTimeSeries при запросе серии моментального снимка.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|metricName|Строка|Имя метрик, для которой запрашивается серия времени.|
|startDateTime|DateTimeOffset|Время начала запрашиваемой серии.|
|endDateTime|DateTimeOffset|Время окончания запрашиваемой серии. Необязательный; если не указано, используется текущее время.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeSeriesParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeSeriesParameter",
  "metricName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```



