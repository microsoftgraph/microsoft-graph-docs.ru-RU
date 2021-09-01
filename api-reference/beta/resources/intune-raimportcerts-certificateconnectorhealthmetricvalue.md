---
title: тип ресурса certificateConnectorHealthMetricValue
description: Значение моментального снимка метрики возвращается в ответ на запрос GetHealthMetricTimeSeries.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91432e5b732c84ca9b94ffbe3f89934d1ac40416
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788764"
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



