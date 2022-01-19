---
title: тип ресурса serviceHealth
description: Представляет сведения о состоянии здоровья службы.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: f44a226375afa5af22b3413d84c47dd34dd473c8
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072504"
---
# <a name="servicehealth-resource-type"></a>тип ресурса serviceHealth

Пространство имен: microsoft.graph

Представляет сведения о состоянии здоровья службы, подписанной клиентом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|Извлечение свойств и связей объекта [serviceHealth.](../resources/servicehealth.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID службы.|
|service|String|Имя службы. Используйте операцию [healthOverviews списка,](../api/serviceannouncement-list-healthoverviews.md) чтобы получить точные имена строк для служб, подписываемых клиентом.|
|status|serviceHealthStatus|Покажите состояние состояния службы overral. Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` . Дополнительные сведения см. [в материале serviceHealthStatus values.](../resources/servicehealthissue.md#servicehealthstatus-values)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|проблемы|[Collection(serviceHealthIssue)](../resources/servicehealthissue.md)|Коллекция проблем, которые произошли в службе, с подробными сведениями по каждой проблеме.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```

