---
title: Тип ресурса assignmentFilterEvaluationSummary
description: Представляем сводку результатов для оценки фильтра назначений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f2e93f481f0b21689b1a83d63f4540c22f50cb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160900"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a>Тип ресурса assignmentFilterEvaluationSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляем сводку результатов для оценки фильтра назначений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignmentFilterId|String|Уникальный идентификатор объекта фильтра назначений|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|Время последнего изменения фильтра назначений.|
|assignmentFilterDisplayName|String|Имя фильтра назначений, определенное администратором.|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Платформа, для которой создается фильтр назначений. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|evaluationResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|Результат оценки фильтра назначений. Возможные значения: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.|
|evaluationDateTime|DateTimeOffset|Был оценен фильтр назначения времени.|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Указать тип фильтра, включаемого или исключаемого. Возможные значения: `none`, `include`, `exclude`.|

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
  "assignmentFilterType": "String"
}
```




