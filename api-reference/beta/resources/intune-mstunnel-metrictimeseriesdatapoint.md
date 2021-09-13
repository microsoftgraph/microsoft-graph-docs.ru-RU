---
title: тип ресурса metricTimeSeriesDataPoint
description: Точка данных серии "Метрики"
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c550f145d99b82307f1ec3ed88040ff1c2357609
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068699"
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

## <a name="relationships"></a>Отношения
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



