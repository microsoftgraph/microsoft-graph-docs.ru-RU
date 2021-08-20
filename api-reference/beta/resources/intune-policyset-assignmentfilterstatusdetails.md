---
title: тип ресурса assignmentFilterStatusDetails
description: Представляем сведения о состоянии для устройства и полезной нагрузки и всех связанных с ними прикладных фильтров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d306c1b0d05e2418653e37737c33f52514be39c4
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266186"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a>тип ресурса assignmentFilterStatusDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляем сведения о состоянии для устройства и полезной нагрузки и всех связанных с ними прикладных фильтров.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managedDeviceId|Строка|Уникальный идентификатор для объекта устройства.|
|payloadId|Строка|Уникальный идентификатор для объекта полезной нагрузки.|
|userId|String|Уникальный идентификатор для объекта UserId. Может быть null|
|свойства устройств|Коллекция [keyValuePair](../resources/intune-policyset-keyvaluepair.md)|Свойства устройства, используемые для оценки фильтра во время регистрации устройства.|
|evalutionSummaries|[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection|Сводки результатов оценки для каждого фильтра, связанного с устройством и полезной нагрузкой|

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
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




