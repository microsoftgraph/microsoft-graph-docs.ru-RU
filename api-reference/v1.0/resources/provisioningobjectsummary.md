---
title: тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d9852745ed14cacd47389da5031cb83af306e2d0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241553"
---
# <a name="provisioningobjectsummary-resource-type"></a>тип ресурса provisioningObjectSummary

Пространство имен: microsoft.graph


Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами. 

## <a name="methods"></a>Методы

| Метод  | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | Получите список всех событий, которые произошли в клиенте. |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|provisioningAction|provisioningAction|Указывает имя действия или имя операции. Возможные значения: `create` `update` , , , , , `delete` `stageddelete` и `disable` `other` `unknownFutureValue` . Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.|
|activityDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|changeId|Строка|Уникальный ID этого изменения в этом цикле.|
|cycleId|Строка|Уникальный ID для итерации задания.|
|durationInMilliseconds|Int32|Указывает, сколько времени потребовалось для завершения этого действия по подготовкам. Измеряется в миллисекунд.|
|id|String| Указывает уникальный идентификатор для действия. Это GUID только для чтения.|
|initiatedBy|[initiator](initiator.md)|Сведения о том, кто инициировал это подготовка.|
|jobId|Строка|Уникальный ID для всего задания по подготовкам.|
|modifiedProperties|[измененная коллекцияProperty](modifiedproperty.md)|Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.|
|provisioningSteps|[provisioningStep](provisioningstep.md) collection|Сведения о каждом шаге в области подготовка.|
|servicePrincipal|Коллекция [servicePrincipal](provisioningserviceprincipal.md)|Представляет принцип службы, используемый для обеспечения.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о предварительном предоставлении объекта-источника.|
|sourceSystem|[provisioningSystem](provisioningsystem.md)|Сведения о исходных системах объекта, который был закамут.|
|provisioningStatusInfo|[provisioningStatusInfo](provisioningstatusinfo.md)|Сведения о состоянии подготовка.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о предварительном предоставлении целевого объекта.|
|targetSystem|[provisioningSystem](provisioningsystem.md)|Сведения о целевой системе объекта.|
|tenantId|String|Уникальный ID клиента Azure AD.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


