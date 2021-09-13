---
title: тип ресурса serviceHealth
description: Представляет сведения о состоянии здоровья службы.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 7bb482f9432de580498ecf7d248c3d9f16abd2a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019134"
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
|status|serviceHealthStatus|Покажите состояние состояния службы overral. Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` .|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|проблемы|[Collection(serviceHealthIssue)](../resources/servicehealthissue.md)|В службе произошел набор проблем с подробными сведениями по каждой проблеме.|

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

