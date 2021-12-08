---
title: тип ресурса certificateConnectorHealthMetricValue
description: Значение моментального снимка метрики возвращается в ответ на запрос GetHealthMetricTimeSeries.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6201f79b302378d1452284ed52d14dab4eccc94
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341007"
---
# <a name="certificateconnectorhealthmetricvalue-resource-type"></a>тип ресурса certificateConnectorHealthMetricValue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значение моментального снимка метрики возвращается в ответ на запрос GetHealthMetricTimeSeries.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dateTime|DateTimeOffset|Timestamp для этой метрической точки данных.|
|successCount|Int64|Количество успешных запросов/операций.|
|failureCount|Int64|Количество сбойных запросов/операций.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorHealthMetricValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorHealthMetricValue",
  "dateTime": "String (timestamp)",
  "successCount": 1024,
  "failureCount": 1024
}
```




