---
title: тип ресурса timeSeriesParameter
description: Параметр передается в GetHealthMetricTimeSeries при запросе серии моментального снимка.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3110404b04bbea136bc242ab52fd87cdb9f502a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080669"
---
# <a name="timeseriesparameter-resource-type"></a>тип ресурса timeSeriesParameter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр передается в GetHealthMetricTimeSeries при запросе серии моментального снимка.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|metricName|String|Имя метрик, для которой запрашивается серия времени.|
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



