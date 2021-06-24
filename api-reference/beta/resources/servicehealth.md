---
title: тип ресурса serviceHealth
description: Представляет сведения о состоянии здоровья службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c11750bbffe64315c6263a26d7dbab333f42b7cf
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109238"
---
# <a name="servicehealth-resource-type"></a>тип ресурса serviceHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии здоровья службы.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|Извлечение свойств и связей объекта [serviceHealth.](../resources/servicehealth.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID службы.|
|service|String|Имя службы.|
|status|serviceHealthStatus|Покажите состояние состояния службы overral. Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` .|

## <a name="relationships"></a>Отношения
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

