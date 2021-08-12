---
title: тип ресурса serviceHealth
description: Представляет сведения о состоянии здоровья службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 254702516d536617ef5afa114bc7a41761ce3499a932b4c7e2d8560ac7f92441
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195617"
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
|id|String|ID службы.|
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

