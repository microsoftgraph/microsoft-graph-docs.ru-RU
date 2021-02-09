---
title: Тип ресурса assignmentFilterStatusDetails
description: Представляет сведения о состоянии для устройства и полезной нагрузки, а также всех связанных примененных фильтров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a376b1ff3d554753120860f1d3541f7952dd6130
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160897"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a>Тип ресурса assignmentFilterStatusDetails

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сведения о состоянии для устройства и полезной нагрузки, а также всех связанных примененных фильтров.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managedDeviceId|String|Уникальный идентификатор объекта устройства.|
|payloadId|String|Уникальный идентификатор объекта полезной нагрузки.|
|userId|String|Уникальный идентификатор объекта UserId. Может иметь null|
|deviceProperties|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Свойства устройства, используемые для оценки фильтра во время регистрации устройства.|
|evalutionSummaries|[Коллекция assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)|Сводка результатов оценки для каждого фильтра, связанного с устройством и полезной нагрузкой|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String"
    }
  ]
}
```




