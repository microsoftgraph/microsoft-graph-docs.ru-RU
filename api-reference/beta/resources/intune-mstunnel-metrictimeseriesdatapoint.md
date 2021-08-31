---
title: тип ресурса metricTimeSeriesDataPoint
description: Точка данных серии "Метрики"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4939450d7cc4a8a42d804a3ccbceb4bfc9fdb297
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800107"
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



