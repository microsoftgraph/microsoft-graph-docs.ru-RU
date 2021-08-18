---
title: тип ресурса assignmentFilterEvaluationSummary
description: Представляем сводку результатов для оценки фильтра назначения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 47a3fdcb4275c55578fd154366563dcc9714512b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58248146"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a>тип ресурса assignmentFilterEvaluationSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляем сводку результатов для оценки фильтра назначения

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignmentFilterId|String|Уникальный идентификатор для объекта фильтра назначения|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|Время последнего изменения фильтра назначения.|
|assignmentFilterDisplayName|String|Имя администратора для фильтра назначения.|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Платформа, для которой создается фильтр назначения. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|assessmentResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|Результат оценки фильтра назначения. Возможные значения: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.|
|assessmentDateTime|DateTimeOffset|Был оценен фильтр назначения времени.|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Указать тип фильтра либо включить, либо исключить. Возможные значения: `none`, `include`, `exclude`.|
|assignmentFilterTypeAndEvaluationResults|[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection|Коллекция типов фильтров и их соответствующих результатов оценки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
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
```




